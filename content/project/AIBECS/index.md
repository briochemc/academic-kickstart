---
title: AIBECS
summary: The ideal tool for exploring global marine biogeochemical cycles.
tags:
- Oceanography
- Julia
- AD
- AIBECS
date: "2019-05-16T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart
  preview_only: true

links:
- icon: github
  icon_pack: fab
  name: Source code
  url: https://github.com/briochemc/AIBECS.jl
url_code: ""
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

<a href="https://github.com/briochemc/AIBECS.jl">
  <img src="https://user-images.githubusercontent.com/4486578/60554111-8fc27400-9d79-11e9-9ca7-6d78ee89ea70.png" alt="logo" title="The AIBECS logo: It represents three global marine biogeochemical cycles, where each element affects the others" align="center" width="100%"/>
</a>


**AIBECS** (for **A**lgebraic **I**mplicit **B**iogeochemical **E**lemental **C**ycling **S**ystem, pronounced like the cool [ibex](https://en.wikipedia.org/wiki/Ibex)) is a Julia package that provides ocean biogeochmistry modelers with an easy-to-use interface for creating and running models of the ocean system.

Simply chose some biogeochemical tracers, define their interactions, and select an ocean circulation, and *Voilà!* — your model is ready to run.

## Getting started


Head over to the [documentation](https://briochemc.github.io/AIBECS.jl/stable/) and find your way to some simple Jupyter notebooks to get you started with AIBECS!


## The Maths

AIBECS represents global biogeochemical cycles with a discretized system of nonlinear partial differential equations that takes the generic form

$$\frac{\partial \boldsymbol{x}}{\partial t} = \boldsymbol{F}(\boldsymbol{x},\boldsymbol{p})$$

where $\boldsymbol{x}$ is a column vector of the model state variables (i.e., the tracers) and $\boldsymbol{p}$ is a vector of model parameters.
(For now, AIBECS only handles steady-state models, for which $\boldsymbol{F}$ does not depend on time.)

This package was developed for models to exploit techniques from linear algebra.
A typical example is if the model is linear (affine), i.e., if

$$\boldsymbol{F}(\boldsymbol{x},\boldsymbol{p}) = \mathbf{A} \, \boldsymbol{x} + \boldsymbol{b}$$

In that case, the model's steady state solution can be computed in a single matrix inversion (via the backslash in MATLAB or Julia), $\boldsymbol{s} = -\mathbf{A}^{-1} \, \boldsymbol{b}$.

However, AIBECS also works for nonlinear problems, i.e., when $\boldsymbol{F}(\boldsymbol{x},\boldsymbol{p})$ is nonlinear, covering a much larger range of models!
In this case, AIBECS uses a state-of-the-art Newton-type solver to find the steady-state solution for you, which is much faster than time-stepping the system until it reaches equilibrium.
(See, e.g., the work of C. T. Kelley.)

The AIBECS also plays well with the [F1Method](https://github.com/briochemc/F1Method.jl) package, which means that it is ideal for efficient, offline optimization of any biogeochemistry model!



