---
title: HTML UI element extraction
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%">Prasang Gupta, <a href="https://www.linkedin.com/in/vishakhabansal91/" target="_blank">Vishakha Bansal</a></span>
summary: Extracted HTML UI elements from wireframe drawings of websites and website screenshots using advanced image pre-processing and confidence cutoff variation. <span style="color:#33cc33;font-style:bold;font-size:120%">Achieved $2^{nd}$ rank in the hackathon</span>.
tags:
- HTML
- UI
- Image Processing
- Deep Learning
- OpenCV
- YOLOv5
- AICrowd
- Hackathon
- ML-DL

date: "2021-07-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: DrawnUI element detection
  focal_point: Smart

links:
- name: Publication
  url: publication/clef2021
url_code: ""
url_pdf: ""
url_slides: "https://docs.google.com/presentation/d/1ihSdVTljhtNBSJ7HZbK8BwW1NHWc6De-"
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

<span style="color:#33cc33">We achieved</span> <span style="color:#33cc33;font-style:bold;font-size:120%">$2^{nd}$ rank</span> <span style="color:#33cc33">in the hackathon.</span>

<span style="font-style:bold;font-size:120%"><a class="mt-1">AIM</a></span>

The aim of this hackathon was to localise and identify several different HTML UI elements in hand-drawn wireframe drawings of websites as well as for screenshots of real websites.

<span style="font-style:bold;font-size:120%"><a class="mt-1">DETAILS</a></span>

The dataset provided for the hackathon contained about 3200 wireframe drawings of websites. The goal was to identify the different HTML UI elemnents present in the image, such as "Text Box", "Button", "Image", etc. Hence, it boiled down to an object detection problem. It also included another dataset containing screenshots of real websites. The problem remained the same for both the datasets.

We used several different Object Detection techniques and decided on using the just released SOTA model YOLOv5. We tried different flavours of YOLOv5 and since inference time was not a bar, we went ahead with the XL version of the same to boost performance. We also used pre-trained weights and performed a LR scheduler study to boost the scores even further.

We also observed that our model was giving out good predictions for the common elements with high confidences, but was not giving outputs for the more uncommon elements. Hence, we performed a study to change the confidence cutoff levels to optimise it for the use case and adjust it according to the distribution in the data. This allowed us to achieve near-perfect performance level of 0.95 F1 score on the validation set.

<span style="font-style:bold;font-size:120%"><a class="mt-1">IMPACT</a></span>

The solution built was performing really good on unseen test images managing an mAP value of 0.82. This model was later swapped with the last year's model in the already developed pipeline to allow rapid prototyping of websites and dashboards.