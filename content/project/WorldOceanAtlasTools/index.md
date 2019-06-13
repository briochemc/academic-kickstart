---
title: World Ocean Atlas Tools
summary: "WorldOceanAtlasTools.jl: A Julia package for data from the World Ocean Atlas."
tags:
- Oceanography
- Julia
- AIBECS
date: "2019-03-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: ""
  focal_point: ""
  preview_only: true

links:
- icon: github
  icon_pack: fab
  name: Source code
  url: https://github.com/briochemc/WorldOceanAtlasTools.jl
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

<a href="https://github.com/briochemc/WorldOceanAtlasTools.jl">
  <img src="https://user-images.githubusercontent.com/4486578/59411626-07e2ed00-8dff-11e9-8daf-e823f61124d9.png" width="100%" align="center">
</a>

[WorldOceanAtlasTools.jl](https://github.com/briochemc/WorldOceanAtlasTools.jl) was developed for the purpose of downloading and using data from the World Ocean Atlas (WOA) database to be used by the [AIBECS.jl](https://github.com/briochemc/AIBECS.jl) package.
The more generic ambition is for [WorldOceanAtlasTools.jl](https://github.com/briochemc/WorldOceanAtlasTools.jl) to provide an API that can fetch data from [this list](https://www.nodc.noaa.gov/OC5/indprod.html) of WOA data sets and products (located on the National Oceanic and Atmospheric Administration (NOAA) wesbite) and fit it to any model's grid.

This is a work in progress, therefore PRs, suggestions, and generally help are, of course, more than welcome!

[WorldOceanAtlasTools.jl](https://github.com/briochemc/WorldOceanAtlasTools.jl) essentially defines the nomenclature and URLs used by the WOA and then relies on the [DataDeps.jl](https://github.com/oxinabox/DataDeps.jl) package developed by [White et al. (2018)](https://arxiv.org/abs/1808.01091) to download the corresponding NetCDF files.
(NetCDF files are read using the [NCDatasets.jl](https://github.com/Alexander-Barth/NCDatasets.jl) package.)

In order to facilitate the use of WOA data in [AIBECS.jl](https://github.com/briochemc/AIBECS.jl), the [WorldOceanAtlasTools.jl](https://github.com/briochemc/WorldOceanAtlasTools.jl) package can use a `grid` from the [OceanGrids.jl](https://github.com/briochemc/OceanGrids.jl) package and bin a WOA tracer into that grid, and uses the [NearestNeighbors.jl](https://github.com/KristofferC/NearestNeighbors.jl) package to decide where to bin each observation.

If you use this package, please cite it using the [CITATION.bib](./CITATION.bib) file, and cite the WOA references using the `citation` function or use the corresponding bibtex entries in the [CITATION.bib](./CITATION.bib) file. 

