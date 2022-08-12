---
title: Active Learning
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%">Prasang Gupta, <a href="https://www.linkedin.com/in/waqar-sarguroh-b53a9982/" target="_blank">Waqar Sarguroh</a></span>
summary: Explored Active Learning with different querying strategies on CIFAR10 dataset and managed to achieve high accuracies with very limited training data
tags:
- Deep Learning
- Active Learning
- CIFAR10
- Proof of Concept
- ML-DL

date: "2019-11-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Active learning flow
  focal_point: Smart

links:
- icon: 
  icon_pack: 
  name: Data
  url: https://www.cs.toronto.edu/~kriz/cifar.html
url_code: ""
url_pdf: ""
url_slides: "https://drive.google.com/file/d/1sh_Z4zjFPV9Pown8UiY6Gatb9ZgGBHgP/view?usp=sharing"
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

<span style="color:#5DADE2;font-style:bold;font-size:120%">AIM</span>

The aim of the study was to build out a pipeline for active learning that other projects with scarce labelled data will leverage for model building. It also included trying the effectiveness of active learning on a standard dataset and evaluate different techniques.

<span style="color:#5DADE2;font-style:bold;font-size:120%">DETAILS</span>

The dataset chosen for this study was CIFAR10. This dataset contains 60,000 32x32 images with 10 unique classes. We used a maximum of 10,000 images at each time for training purposes. This study's focus was to compare the performance of active and passive learning using same number of labelled samples. 

The passive learning model would be trained on a uniform distribution of the dataset size, however, the active learning model would be initialised with half the training size and then would be trained for the full size by sequential queries. We tried 3 queries in this study : uncertainty, margin sampling and entropy sampling. We achieved better performance with active learning for all the sizes, however, the improvement in performance varied from as low as 1% to a sizable 23%. The details for all the experiments and the queries can be seen in the slides.

<span style="color:#5DADE2;font-style:bold;font-size:120%">IMPACT</span>

The pipeline developed from this project was consecutively used in multiple client projects to improve the modelling capabilities and thrive wherever manually labelling the full dataset was not an option.