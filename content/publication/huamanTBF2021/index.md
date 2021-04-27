---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Towards Knowledge Graphs Validation through Weighted Knowledge Sources"
authors: ["Elwin Huaman", "Amar Tauqeer", "Geni Bushati", "Anna Fensel"]
date: 2021-04-26T01:57:51+01:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2021-04-26T01:57:51+01:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "arXiv"
publication_short: ""

abstract: "The performance of applications, such as personal assistants, search engines, and question-answering systems, rely on high-quality knowledge bases, a.k.a. Knowledge Graphs (KGs). To ensure their quality one important task is Knowledge Validation, which measures the degree to which statements or triples of a Knowledge Graph (KG) are correct. KGs inevitably contains incorrect and incomplete statements, which may hinder the adoption of such KGs in business applications as they are not trustworthy.
In this paper, we propose and implement a validation approach that computes a confidence score for every triple and instance in a KG. The computed score is based on finding the same instances across different weighted knowledge sources and comparing their features.
We evaluated the performance of our Validator by comparing a manually validated result against the output of the Validator.
The experimental results showed that compared with the manual validation, our Validator achieved as good precision as the manual validation, although with certain limitations.
Furthermore, we give insights and directions toward a better architecture to tackle KG validation."

# Summary. An optional shortened abstract.
summary: "A knowledge graph validation approach that computes a confidence score for every triple and instance in a KG"

tags: ["Research", "Knowledge Graphs"]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: https://arxiv.org/pdf/2104.12622.pdf
url_code:
url_dataset:
url_poster:
url_project:
url_slides:
url_source: https://arxiv.org/abs/2104.12622
url_video:

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: [WordLiftNG]

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
