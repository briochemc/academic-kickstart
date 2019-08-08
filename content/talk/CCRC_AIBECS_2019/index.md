---
title: >
  Introducing AIBECS.jl, a Julia package for creating global marine biogeochemistry models
event: CCRC Seminar Series
event_url: http://www.ccrc.unsw.edu.au/events/benoit-pasquier-introducing-aibecsjl-julia-package-creating-global-marine-biogeochemistry
location: Climate Change Research Centre (CCRC), UNSW, Australia
summary:
abstract: >
  Running standard global marine biogeochemistry models comes with large computational costs and with a steep learning curve. The recently developed AWESOME OCIM (for A Working Environment for Simulating Ocean Movement and Elemental cycling in an Ocean Circulation Inverse Model) is an attractive alternative because it offers better user experience thanks to a MATLAB Graphical User Interface (GUI), and faster computations thanks to the OCIM's steady-state matrix formulation of the ocean circulation. Benoît will introduce and give a live demonstration of the AIBECS (for Algebraic Implicit Biogeochemical Elemental Cycling System), an open-source, user-friendly, fast, and modular Julia package, which aims to provide a solution to the limitations of the AWESOME OCIM. The AIBECS provides an Application Programming Interface (API) to generate global steady-state marine biogeochemistry models in just a few lines of code. Under the hood, the AIBECS comes with state-of-the-art nonlinear-system solvers, auto-differentiation algorithms, and was designed with parameter optimization/estimation and uncertainty analysis in mind. The AIBECS allows researchers to focus on the science rather than spending time reinventing the wheel for differentiating convoluted systems, for solving nonlinear problems, or for leveraging cryptic linear-algebra shortcuts. Because of its ease of use, the AIBECS is ideal for teaching and exploratory research. The AIBECS is also ideal for cutting-edge research owing to its open-source design, its modularity, its advanced algorithms, and its novel-diagnostic capabilities.



# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2019-08-07"
#date_end: "2014-10-01T10:45:00Z"
all_day: true

# Schedule page publish date (NOT talk date).
#publishDate: "2014-09-01T00:00:00Z"

authors:
- admin
- François Primeau
- J. Keith Moore
tags: []

# Is this a featured talk? (true/false)
featured: false

image:
  caption: ''
  focal_point: Right
  preview_only: true

#links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
#url_code: ""
#url_pdf: ""
url_slides: "https://nbviewer.jupyter.org/format/slides/github/briochemc/AIBECS_demos/blob/master/presentations/CCRC_Seminar_20190807_safe.ipynb#/"
#url_video: ""

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
#projects:
#- internal-project

# Enable math on this page?
math: true
---

