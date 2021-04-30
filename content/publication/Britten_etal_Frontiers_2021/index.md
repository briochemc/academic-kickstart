---
title: "Evaluating the Benefits of Bayesian Hierarchical Methods for Analyzing Heterogeneous Environmental Datasets: A Case Study of Marine Organic Carbon Fluxes"
authors:
- "[Gregory L. Britten](http://www.gregorybritten.info/home)"
- "[Yara Mohajerani](https://yaramohajerani.github.io/)"
- Louis Primeau
- "[Murat Aydin](https://www.ess.uci.edu/people/maydin)"
- "[Catherine Garcia](https://www.ess.uci.edu/people/catgar)"
- "[Weilei Wang](https://www.ess.uci.edu/people/weileiw)"
- admin
- "[Barry B. Cael](http://paocweb.mit.edu/people/bcaelb)"
- "[François W. Primeau](https://www.ess.uci.edu/people/fprimeau)"
date: "2021-01-01T00:00:00Z"
doi: "10.3389/fenvs.2021.491636"

# Schedule page publish date (NOT publication's date).
publishDate: "2019-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*Frontiers in Environmental Science*"
publication_short: ""

abstract: Large compilations of heterogeneous environmental observations are increasingly available as public databases, allowing researchers to test hypotheses across datasets. Statistical complexities arise when analyzing compiled data due to unbalanced spatial sampling, variable environmental context, mixed measurement techniques, and other reasons. Hierarchical Bayesian modeling is increasingly used in environmental science to describe these complexities, however few studies explicitly compare the utility of hierarchical Bayesian models to simpler and more commonly applied methods. Here we demonstrate the utility of the hierarchical Bayesian approach with application to a large compiled environmental dataset consisting of 5,741 marine vertical organic carbon flux observations from 407 sampling locations spanning eight biomes across the global ocean. We fit a global scale Bayesian hierarchical model that describes the vertical profile of organic carbon flux with depth. Profile parameters within a particular biome are assumed to share a common deviation from the global mean profile. Individual station-level parameters are then modeled as deviations from the common biome-level profile. The hierarchical approach is shown to have several benefits over simpler and more common data aggregation methods. First, the hierarchical approach avoids statistical complexities introduced due to unbalanced sampling and allows for flexible incorporation of spatial heterogeneitites in model parameters. Second, the hierarchical approach uses the whole dataset simultaneously to fit the model parameters which shares information across datasets and reduces the uncertainty up to 95% in individual profiles. Third, the Bayesian approach incorporates prior scientific information about model parameters; for example, the non-negativity of chemical concentrations or mass-balance, which we apply here. We explicitly quantify each of these properties in turn. We emphasize the generality of the hierarchical Bayesian approach for diverse environmental applications and its increasing feasibility for large datasets due to recent developments in Markov Chain Monte Carlo algorithms and easy-to-use high-level software implementations.

# Summary. An optional shortened abstract.
summary:

tags:

featured: true

# links:
# - name: ""
#   url: ""
url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'The directed acyclic graph (DAG) structure of the Bayesian hierarchical model — see [*Britten et al.*, 2021](https://doi.org/10.3389/fenvs.2021.491636)'
  focal_point: ""
  preview_only: true

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---


