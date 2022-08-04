---
title: Active Learning
subtitle: 
summary: Explored Active Learning with different querying strategies on CIFAR10 dataset and managed to achieve high accuracies with very limited training data
tags:
- Deep Learning
- Active Learning
- CIFAR10

date: "2020-12-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Damage segmentation on a sample image
  focal_point: Smart

links:
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
The aim of the study was to try the effectiveness of active learning for cases where labelled data is scarce. The dataset chosen for this study was CIFAR10. This dataset contains 60,000 images of size 32x32 with 10 classes. The images are single label and are mutually exclusive from each other. We have used a maximum of 10,000 images at each time for trainig purposes.

This study's focus was to compare the performance of active and passive learning on the same dataset size. The passive learning model would be trained on a uniform distribution of the dataset size, however, the active learning model would be initialised with half the training size and then would be trained for the full size by sequential queries. We have tried 3 queries in this study : uncertainty, margin sampling and entropy sampling. We achieved better performance with active learning for all the sizes, however, the difference between the performance of the two varied depending on the total size of the dataset going from as low as 1% to a sizable 23%. The details for all the experiments and the queries can be seen in the slides.
