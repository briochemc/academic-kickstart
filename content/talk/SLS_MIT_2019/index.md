---
title: >
  Developing a new, open-source, user-friendly, fast, modular, global marine biogeochemistry model (in Julia)
event: Oceanography and Climate Sack Lunch Seminar
event_url: http://paoc.mit.edu/paoc/events/seminars/SLS.htm
location: Massachussets Institute of Technology, Cambridge, Massachussets, USA
summary:
abstract: >
  One of the most successful tools made available to oceanographers recently is the Ocean Data View (ODV) software, used "for the analysis and visualization of oceanographic and meteorological data sets." Part of the success of ODV comes from its simplicity, which makes it attractive to oceanographers. Current global marine biogeochemistry models, on the other hand, lack this appeal and generally come with a steep learning curve. So steep, in fact, that very few non-modelers ever use these models on their own and computational tasks are delegated to collaborating model experts. This problematic barrier to entry in modeling, which hinders the progress of oceanography, has recently been lowered with the release of the AWESOME OCIM (A Working Environment for Simulating Ocean Movement and Elemental cycling in an Ocean Circulation Inverse Model, or AO), a software with a graphical user interface (GUI) for modeling a single biogeochemical tracer, using — under the hood — linear algebra.< \br>

  Here I will present some work in progress for developing a new marine biogeochemistry model that builds on the ideas behind the AO and provides users with an open-source, user-friendly, fast, and modular software. Among other goals, this model aims to allow users to represent the coupling of multiple tracers (such as dissolved iron (DFe) and macronutrients) that can be embedded in different models of the ocean's circulation (e.g., swap in the OCIM transport with an average of the MITgcm circulation). The model also addresses a number of features that are currently absent in the AO, like the ability to represent non-linear mechanisms (such as the scavenging of DFe by sinking particles). Additionally, a powerful feature of the OCIM that is not leveraged by the AO is its computational speed, which allows for objective parameter optimization and sensitivity analysis. Most of the model's capabilities stem from the language it is developed in, the Julia language, which is a free, open-source, general-purpose, and fast alternative to MATLAB (the language in which the AO is written).

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2019-01-24"
#date_end: "2014-10-01T10:45:00Z"
all_day: true

# Schedule page publish date (NOT talk date).
#publishDate: "2014-09-01T00:00:00Z"

authors:
- admin
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

