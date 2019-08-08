---
title: >
  F-1 algorithm: Efficient differentiation through large steady-state problems
event: Applied Mathematics Seminar
event_url: https://www.science.unsw.edu.au/events/f-1-algorithm-efficient-differentiation-through-large-steady-state-problems
location: School of Mathematics and Statistics, UNSW, Australia
summary:
abstract: >
  Introducing a Julia package to efficiently differentiate an objective function defined implicitly by the solution of a large PDE system.<br>
  
  Steady-state systems of nonlinear partial differential equations (PDEs) are common in engineering and the biogeosciences. These systems are typically controlled by parameters that can be estimated efficiently using second-order optimization algorithms. However, computing the gradient vector and Hessian matrix of a given objective function defined implicitly by the solution of large PDE systems is seldom economical.<br>
  
  A fast and easy-to-use algorithm is introduced for computing the gradient and Hessian of an objective function implicitly constrained by a steady-state PDE system. The algorithm, which is based on the use of hyperdual numbers, is called the F-1 algorithm, because it requires only one factorization of the constraint-equation Jacobian. Careful examination of the relationships that arise from differentiating the PDE system reveal analytical shortcuts that the F-1 algorithm leverages. Benchmarks of the F-1 algorithm against five numerical differentiation schemes are shown in the context of optimizing a global steady-state model of the marine phosphorus cycle that depends explicitly on <i>m</i>=6 parameters. In this context, the F-1 algorithm computes the Hessian 16 to 100 times faster than other algorithms, allowing for the entire optimization procedure to be performed 4 to 26 times faster. This is because other algorithms require O(<i>m</i>) to O(<i>m</i>²) factorizations, which suggests even greater speedups for larger problems.<br>
  
  A live demonstration of using the F-1 algorithm, which is implemented as a Julia package, is given.



# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2019-08-08"
#date_end: "2014-10-01T10:45:00Z"
all_day: true

# Schedule page publish date (NOT talk date).
#publishDate: "2014-09-01T00:00:00Z"

authors:
- admin
- François Primeau
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
url_slides: "https://nbviewer.jupyter.org/format/slides/github/briochemc/F1_demos/blob/master/presentations/UNSW_AppliedSeminar_20190808_safe.ipynb#/"
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

