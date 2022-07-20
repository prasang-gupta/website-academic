---
title: Demand Prediction with Competition Analysis
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%">Prasang Gupta, <a href="https://www.linkedin.com/in/amitoj-singh94/" target="_blank">Amitoj Singh</a>, <a href="https://www.linkedin.com/in/shazhoda/" target="_blank">Shaz Hoda</a></span>
summary: Predicted demand using data from competition and other variables such as demographic and footfall variations in the region.
tags:
- Deep Learning
- Active Learning
- CIFAR10
- Proof of Concept
- ML-DL

date: "2020-11-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Damage segmentation on a sample image
  focal_point: Smart

links:
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

<span style="color:#5DADE2;font-style:bold;font-size:120%">AIM</span>

The aim of this study was to predict consumer demand using data from competition and infusing it with other datasets that influence demand like mobility and demographic variables. The other goal was to correct a proprietary mobility dataset used by PwC to incorporate for mobility changes brought on by COVID restrictions.

<span style="color:#5DADE2;font-style:bold;font-size:120%">DETAILS</span>

The proprietary dataset mentioned had several flaws including data inconsistencies over months and years and noisy data which was not helping in developing stable models. It also didn't account for any socio-economic variables based on the demographics of the region. To correct this, the proprietary dataset was merged with demographics variables based on the location and some feature engineering was done to get the mobility in radii of 1km to 5km based on the store location. The final sales value was kept as the dependent field for the model.

Multiple model architectures were tried to model this information to correct the mobility, including ML and DL models. Finally, a voting ensemble method was selected which was modelling the corrected demand with an accuracy of about 70%.

To bump up the numbers further, an aerial snapshot of the region around the score was obtained from Google Satellite API at a tuned zoom level and a segmentation exercise was performed on the image to extract the type of region around the store. This was expected to bring another dimension of immediate demographics in the dataset. This was done by extracting the coverage area of different colors based on pixel masks :

- Grey (signifying roads, parking lots, streets, etc)
- Green (signifying agriculture, parks, vegetation, etc)
- White (signifying roof-tops, buildings, etc)

<span style="color:#5DADE2;font-style:bold;font-size:120%">IMPACT</span>

The final model with all the variables included (engineered visits from proprietary data, Google mobility data, demographics data and derived immediate demographics of the store from satellite images) achieved a test accuracy of 75%. This improved the quality of the mobility data and impacted tens of projects that utilised this mobility dataset helping in building much more accurate and robust models for client deliveries.