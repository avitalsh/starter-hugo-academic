---
title: "Render Before Reading: Visual Rendering as a Prompt Injection Defense"
authors:
- Jie Zhang*
- Andrei Baroian*
- Jan N. van Rijn
- admin
- Florian Tramèr
# author_notes:
# - "Equal contribution"
# - "Equal contribution"
date: "2026-05-05T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2026-09-28T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["preprint"]

# Publication name and optional abbreviated publication name.
publication: "Preprint"
publication_short: ""

abstract: |
  Large language models are vulnerable to prompt injection attacks, where thirdparty adversarial content can hijack the model’s behavior. In this paper, we study the role played by the adversarial data’s input modality, and identify a systematic asymmetry: multimodal LLMs are more likely to follow adversarial instruction when they appear as text than when the same instruction is delivered through a non-textual channel (e.g., as an image). We hypothesize that this modality gap arises from text-centric instruction tuning, which teaches models to obey textual instructions while treating other modalities mainly as content to parse or describe. We then demonstrate how this gap can be turned into a training-free defense, by rendering all untrusted payloads as typographic images (or audio) before they reach the model. Across ten models and two prompt injection benchmarks (DirectInject and AgentDojo) we show that our defense Pictionary consistently reduces attack success rates even against the strongest adaptive attacks and human red teamers, while largely preserving benign utility. We further show that benign fine-tuning on image-rendered instructions erodes the modality gap, tracing it to the text-centric instruction-tuning distribution. Our code is available at https://github.com/zj-jayzhang/Pictionary.

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
# - Source Themes
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: 'https://arxiv.org/pdf/2609.36121'
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

