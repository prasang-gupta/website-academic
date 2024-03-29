---
title: "UI element detection from wireframe drawings of websites"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.

authors:
- admin
- Vishakha Bansal

# Author notes (optional)
# author_notes:
# - "Equal contribution"
# - "Equal contribution"

date: "2021-07-27T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: 12$^{th}$ International Conference of the CLEF Association (CLEF 2021) - Bucharest, Romania
publication_short: 

abstract: User Interfaces (UIs) wireframe is a crucial part of designing front-end of websites and mobile applications. Detection of UI elements such as paragraphs, buttons, images etc. from the wireframes using advanced Artificial Intelligence (AI) algorithms pave the way to automate the process of conversion of wireframes to Hypertext Mark-up Language (HTML) code. In this paper, we have explored different variants of 5th generation of You Only Look Once (YOLOv5) algorithm and post-processing techniques involving tuning of confidence cut-off variable for detection of UI elements. Our final approach comprises of data pre-processing using contrast normalization and conversion to black and white (BW), detection and localization of UI elements using YOLOv5x variant followed by confidence cutoff for selecting final bounding boxes. This approach resulted in Mean Average Precision (mAP) of 0.836 on the test data.

# Summary. An optional shortened abstract.
summary: <a class="mt-1">12$^{th}$ International Conference of the CLEF Association (CLEF 2021) - Bucharest, Romania</a>

tags: ['Website UI elements', 'UI element extraction', 'Image Processing', 'OpenCV', 'Object Detection', 'YOLOv5', 'Confidence Cutoff Variation']

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'http://ceur-ws.org/Vol-2936/paper-101.pdf'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: 'https://docs.google.com/presentation/d/1ihSdVTljhtNBSJ7HZbK8BwW1NHWc6De-'
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'DrawnUI element detection'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- websiteuidetection

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
---
