---
title: Damaged Car Parts Segmentation for auto claims
subtitle: 
summary: Performed damanged car parts segmentation for automating auto claims with additional features like explainability and automated claim / damage report generation
tags:
- Deep Learning
- Semantic segmentation
- Classification
- Auto insurance
- AI assisted claims

date: "2019-09-01T00:00:00Z"

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

* *CLIENT PROBLEM*

The client wanted to reduce the time spent by their employees on looking through several different photographs submitted for insurance claims clearing and ascertain damaged parts of the vehicle with the extent of damage.

* *OUR SOLUTION*

We solved the problem by training a semantic segmentation model used for ascertainining the different kinds of damage that were present in the photograph of a vehicle (like the figure attached). To ensure the correctness of the model, we also employed an explainable AI technique, LIME, which returns the parts of the image it is looking at when coming to a decision about the damage. 

A few classification models were also trained to fetch images which were visually similar with the current image. The different variants were the similar damage model, where the model would return the top images which have visually similar damage to the current image. The other variant was the similar non-damage model, in which the model would return the top images of similar vehicles of previously processed claims. 

To top it all off, an automated report generation tool was coupled with the model (using FPDF), which returned a formatted PDF report having detailed information regarding the damage and the claims.

* *VALUE GENERATED*

The segmentation model ensured that the client team spent lesser time on figuring out the damage and more time providing personalised support to the consumers. The classification models helped the client team to look at some previous claims to decide the outcome for the current claim in a more informed and consistent manner. This improved the overall reputation of the firm in disbursing out claims. Also, the automated report could be handed over to the consumers directly for a much more transparent view into the claims processing.