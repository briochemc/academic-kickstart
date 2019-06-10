---
title: Dual Matrix Tools
summary: DualMatrixTools.jl: A Julia package for solving dual-valued linear systems.
tags:
- Algebra
- Julia
- Automatic Differentiation
- Dual Numbers
date: "2019-05-06T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: 'Solving a dual-valued linear system'
  focal_point: ""
  preview_only: true

links:
- icon: github
  icon_pack: fab
  name: Source
  url: https://github.com/briochemc/DualMatrixTools.jl
url_code: "https://github.com/briochemc/DualMatrixTools.jl"
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

<img src="featured.png" alt="logo" title="logo" align="center" height="400"/>

[DualMatrixTools](https://github.com/briochemc/DualMatrixTools.jl) is a Julia package for solving dual-valued linear systems.

Essentially, it provides an overload for [Julia](https://julialang.org/)'s `factorize` and `\` functions that work with dual-valued arrays.
It uses the dual type defined by the [DualNumbers.jl](https://github.com/JuliaDiff/DualNumbers.jl) package.
The idea is that for a dual-valued matrix

$$M = A + \varepsilon \, B,$$

its inverse is given by

$$M^{-1} = (I - \varepsilon \, A^{-1} \, B) A^{-1}.$$

Therefore, only the inverse of $A$ is required to evaluate the inverse of $M$.
This package makes available a `DualFactors` type which containts (i) the factors of $A$ and (ii) the non-real part, $B$.
It also overloads `factorize` to create an instance of `DualFactors` (when invoked with a dual-valued matrix), which can then be called with `\` to efficiently solve dual-valued linear systems of the type $M \, x = B$.

This package should be useful for autodifferentiation of functions that use `\`.
Note the same idea extends to hyper dual numbers (see the [HyperDualMatrixTools.jl](https://github.com/briochemc/HyperDualMatrixTools.jl) package).

## Usage

1. Create your dual-valued matrix `M`:

    ```julia
    julia> M = A + ε * B
    ```

2. Apply `\` to solve systems of the type `M * x = b`

    - without factorization:

        ```julia
        julia> x = M \ b
        ```

    - or better, with prior factorization:

        ```julia
        julia> Mf = factorize(M)

        julia> x = Mf \ b
        ```

        (This is better in case you want to solve for another `b`!)

## Advanced usage

In the context of iterative processes with multiple factorizations and forward and back substitutions, you may want to propagate dual-valued numbers while leveraging (potentially) the fact the real part of the matrices to be factorized remains the same throughout.
This package provides an in-place `factorize`, with a flag to update (or not) the factors.
Usage is straightforward.
By default, `factorize` does *not* update the factors

```julia
julia> factorize(Mf, M) # only Mf.B is updated
```

If you want to update the real-valued factors too, use

```julia
julia> factorize(Mf, M, update_factors=true) # Mf.B and Mf.Af are updated
```

## Citation

If you use this package, please cite it!
Use the button at the top of this page, or go to the [Zenodo record of the package](https://doi.org/10.5281/zenodo.1493571) and export the citation from there (the "Export" box at the bottom of that page).
