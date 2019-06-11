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


[WorldOceanAtlasTools](https://github.com/briochemc/WorldOceanAtlasTools.jl) was developed for the purpose of downloading and using data from the World Ocean Atlas (WOA) database.
The goal is to provide an API that has access to parts of [this list](https://www.nodc.noaa.gov/OC5/indprod.html) of WOA data sets and products (located on the National Oceanic and Atmospheric Administration (NOAA) wesbite).

This is a work in progress although it is currently used by the [AIBECS.jl](https://github.com/briochemc/AIBECS.jl) package and depending projects.
PRs, suggestions, and generally help are, of course, more than welcome!

WorldOceanAtlasTools essentially defines the nomenclature and URLs used by the World Ocean Atlas and then relies on the [DataDeps.jl](https://github.com/oxinabox/DataDeps.jl) package developed by [White et al. (2018)](https://arxiv.org/abs/1808.01091) to download the corresponding NetCDF files.
(NetCDF files are read using the [NCDatasets.jl](https://github.com/Alexander-Barth/NCDatasets.jl) package.)

If you use this package, please cite it using the [CITATION.bib](./CITATION.bib) file, and cite the WOA references using the `citation` function. 
