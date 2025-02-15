---
title: "Machine Against the RAG: Jamming Retrieval-Augmented Generation with Blocker Documents"
authors:
- admin
- Roei Schuster
- Vitaly Shmatikov
# author_notes:
# - "Equal contribution"
# - "Equal contribution"
date: "2024-06-09T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2025-08-13T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["conference paper"]

# Publication name and optional abbreviated publication name.
publication: "USENIX Security 2025"
publication_short: ""

abstract: |
  Retrieval-augmented generation (RAG) systems respond to queries by retrieving relevant documents from a knowledge database, then generating an answer by applying an LLM to the retrieved documents.
  
  We demonstrate that RAG systems that operate on databases with potentially untrusted content are vulnerable to a new class of denial-of-service attacks we call jamming.  An adversary can add a single ``blocker'' document to the database that will be retrieved in response to a specific query and, furthermore, result in the RAG system not answering the query - ostensibly because it lacks the information or because the answer is unsafe.
  
  We describe and analyze several methods for generating blocker documents, including a new method based on black-box optimization that does not require the adversary to know the embedding or LLM used by the target RAG system, nor access to an auxiliary LLM to generate blocker documents.\nWe measure the efficacy of the considered methods against several LLMs and embeddings, and demonstrate that the existing safety metrics for LLMs do not capture their vulnerability to jamming.  We then discuss defenses against blocker documents.

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
# - Source Themes
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: https://arxiv.org/pdf/2406.05870.pdf
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

