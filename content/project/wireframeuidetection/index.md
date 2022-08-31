---
title: HTML UI element extraction
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%">Prasang Gupta, <a href="https://www.linkedin.com/in/swayambodha-mohapatra-7a7a22110/" target="_blank">Swayambodha Mohapatra</a></span>
summary: Extracted HTML UI elements from wireframe drawings of websites ideating novel multi-pass inference technique to boost recall. <span style="color:#33cc33;font-style:bold;font-size:120%">Achieved $3^{rd}$ rank in the hackathon</span>.
tags:
- HTML
- UI
- Image Processing
- Deep Learning
- OpenCV
- Mask R-CNN
- AICrowd
- Hackathon
- ML-DL

date: "2020-07-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Novel Multi Pass Inference Technique
  focal_point: Smart

links:
- name: Publication
  url: publication/clef2020
url_code: ""
url_pdf: ""
url_slides: "https://docs.google.com/presentation/d/1lugSGraB3toxS0a8JSdKNWV1rhPSED0R"
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

<span style="color:#33cc33">We achieved</span> <span style="color:#33cc33;font-style:bold;font-size:120%">$3^{rd}$ rank</span> <span style="color:#33cc33">in the hackathon.</span>

<span style="font-style:bold;font-size:120%"><a class="mt-1">AIM</a></span>

The aim of this hackathon was to localise and identify several different HTML UI elements in hand-drawn wireframe drawings of websites.

<span style="font-style:bold;font-size:120%"><a class="mt-1">DETAILS</a></span>

The dataset provided for the hackathon contained about 3000 wireframe drawings of websites. The goal was to identify the different HTML UI elemnents present in the image, such as "Text Box", "Button", "Image", etc. Hence, it boiled down to an object detection problem.

We tried using several Object Detection algorithms like YOLO, R-CNN and Mask-RCNN and decided on Mask-RCNN as it was providing us with the best results. However, one thing we observed in our outputs was that our Precision scores were good, but the model was lacking in Recall bringing the whole F1 down. To solve this problem, we came up with a novel technique "Multi-Pass Inference" that booosted our recall scores.

The technique involves running the image through the model multiple times, each time taking note of the objects that are already detected and removing them for subsequent passes. This forced the model to predict more instances of the elements in the image. We smarlty combined the objects detected in multiple passes to overall boost the recall score of our model helping us to take a podium spot in the leaderboard.

<span style="font-style:bold;font-size:120%"><a class="mt-1">IMPACT</a></span>

The solution built was performing really good on unseen test images managing an mAP (IoU > 0.5) score of 64.12. This solution was later implemented into a pipeline to allow rapid prototyping of websites and dashboards.