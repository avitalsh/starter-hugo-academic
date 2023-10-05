---
title: "Beyond Labeling Oracles: What does it mean to steal ML models?"
authors:
- admin
- Ilia Shumailov
- Murat A. Erdogdu
- Nicolas Papernot
# author_notes:
# - "Equal contribution"
# - "Equal contribution"
date: "2023-10-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2023-10-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["conference paper"]

# Publication name and optional abbreviated publication name.
publication: "preprint"
publication_short: ""

abstract: Model extraction attacks are designed to steal trained models with only query access, as is often provided through APIs that ML-as-a-Service providers offer. ML models are expensive to train, in part because data is hard to obtain, and a primary incentive for model extraction is to acquire a model while incurring less cost than training from scratch. Literature on model extraction commonly claims or presumes that the attacker is  able to save on both data acquisition and labeling costs. We show that the attacker often does not. This is because current attacks implicitly rely on the adversary being able to sample from the victim model's data distribution. We thoroughly evaluate factors influencing the success of model extraction. We discover that prior knowledge of the attacker, i.e. access to in-distribution data, dominates other factors like the attack policy the adversary follows to choose which queries to make to the victim model API.  Thus, an adversary looking to develop an equally capable model with a fixed budget has little practical incentive to perform model extraction, since for the attack to work they need to collect in-distribution data, saving only on the cost of labeling. With low labeling costs in the current market, the usefulness of such attacks is questionable.  Ultimately, we demonstrate that the effect of prior knowledge needs to be explicitly decoupled from the attack policy. To this end, we propose a benchmark to evaluate attack policy directly. 

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
# - Source Themes
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: https://arxiv.org/pdf/2310.01959.pdf
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# image:
#  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/jdD8gXaTZsc)'
#  focal_point: ""
#  preview_only: false

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
slides: example
---

