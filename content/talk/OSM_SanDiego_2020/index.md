---
title: >
  AIBECS.jl: the ideal tool for marine biogeochemistry modelling
event: Ocean Sciences Meeting 2020
event_url: https://osm.agu.org/2020/
location: San Diego Convention Center, San Diego, California, USA
summary:
abstract: >
  Progress in global marine biogeochemistry increasingly relies on models. In general, converting conceptual mechanisms into useful numerical simulations comes with large computational costs and significant amounts of time developing code. A recently developed alternative is the AWESOME OCIM (A Working Environment for Simulating Ocean Movement and Elemental cycling in an Ocean Circulation Inverse Model, or AO), which drastically reduces development time with its graphical user interface (GUI). Building on the OCIM's steady-state matrix formulation of the ocean circulation, the AO allows computationally efficient simulations of single tracers controlled by linear mechanisms. Here, we present the AIBECS (for Algebraic Implicit Biogeochemical Elemental Cycling System), an open-source, user-friendly, fast, and modular Julia package, which aims to extend the AO's capabilities to nonlinear, multi-tracer systems, embedded in other circulations than just the OCIM. Instead of a GUI, the AIBECS provides an application programming interface (API) to create global steady-state marine biogeochemistry models in a few lines of code, allowing oceanographers to focus on research instead of wasting precious time reinventing the wheel. Because of its ease of use, the AIBECS is perfect for teaching and exploratory research. Yet, it is designed for cutting-edge research owing to its advanced algorithms and diagnostic capabilities. Under the hood, the AIBECS runs with state-of-the-art nonlinear-system solvers and auto-differentiation algorithms. Combined with highly-efficient parameter optimization or uncertainty analysis tools, it aspires to be at the forefront of global biogeochemistry modeling. In short, the AIBECS is the ideal tool for exploring global marine biogeochemical cycles.


# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2020-02-20"
#date_end: "2014-10-01T10:45:00Z"
all_day: true

# Schedule page publish date (NOT talk date).
#publishDate: "2014-09-01T00:00:00Z"

authors:
- admin
- François Primeau
tags: []

# Is this a featured talk? (true/false)
featured: true

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
#url_slides: ""
#url_video: ""

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example

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

