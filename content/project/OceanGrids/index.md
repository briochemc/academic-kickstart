---
title: Ocean Grids
summary: "OceanGrids.jl: Ocean grids for AIBECS."
tags:
- Julia
- Oceanography
- AIBECS
date: "2019-06-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: "logo"
  focal_point: "Center"
  preview_only: true

links:
- icon: github
  icon_pack: fab
  name: Source code
  url: https://github.com/briochemc/OceanGrids.jl
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

<a href="https://gist.github.com/briochemc/10e891bdb7da49fc4bf5467a5876434f">
  <img src="https://user-images.githubusercontent.com/4486578/59238897-0a004c80-8c43-11e9-861c-5fe00069af92.png", align="center", width="100%">
</a>


This package is a dependency of [AIBECS](https://github.com/briochemc/AIBECS.jl.git).
It defines types for grids used by AIBECS.

The goal of [OceanGrids](https://github.com/briochemc/OceanGrids.jl.git) is to standardize the format of grids in order for AIBECS to avoid confusion when swapping the circulation it uses for another.

For example, units for the grid data in the Ocean Circulation Inverse Model (OCIM, see [*DeVries et al*., 2014](https://doi.org/10.1002/2013GB004739)) products are not documented, so that it is easy to get confused and carry dimensional inconsistencies in one's model.
[OceanGrids](https://github.com/briochemc/OceanGrids.jl.git) attempts to fix these discrepancies by always using the same format and provide tests to ensure some level of consistency.
