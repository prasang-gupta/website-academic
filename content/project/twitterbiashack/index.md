---
title: Twitter Bias Hackathon
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%">Prasang Gupta, <a href="https://www.linkedin.com/in/amitoj-singh94/" target="_blank">Amitoj Singh</a>, <a href="https://www.linkedin.com/in/ilana-golbin-6167373b/" target="_blank">Ilana Golbin</a></span>
summary: Participated in the Twitter Bias Hackathon and highlighted bias instances in Twitter's Saliency model used to crop images building a case study with Tokyo Olympics images as example. <span style="color:#5DADE2;font-style:bold;font-size:120%">Achieved 9th rank in the hackathon</span>.
tags:
- Bias
- Responsible AI
- Deep Learning
- Tokyo Olympics 2022
- Twitter
- Saliency Model
- Hackathon

date: "2021-08-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Simple representation of concept drift sources
  focal_point: Smart

links:
- icon: 
  icon_pack: 
  name: Data
  url: https://github.com/prasang-gupta/twitter-algorithmic-bias
url_code: "https://github.com/prasang-gupta/twitter-algorithmic-bias"
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

<span style="color:#58D68D">We achieved</span> <span style="color:#52BE80;font-style:bold;font-size:120%">9th rank</span> <span style="color:#58D68D">in the hackathon.</span>

<span style="color:#5DADE2;font-style:bold;font-size:120%">AIM</span>

The aim of the hackathon was to higlight bias in Twitter's Saliency model.

<span style="color:#5DADE2;font-style:bold;font-size:120%">DETAILS</span>

Twitter's Saliency model is a model that is used to crop over-sized images to fit on the screen representing a thumbnail preview. The saliency model is responsible for selecting the most "salient" part of the image and that part is consequently kept in the thumbnail and the area surroinding it is cropped off.

We decided to chose, recently concluded at the time, Tokyo Olympics 2022 as a case study for highlighting bias. We downloaded around 5000 images across 10 different sports and ran the saliency model on top of them. We also passed these images through an object detection model to identify images with and without athletes.

We ran several studies, the main being classifying the images and the crops as something that was biased or not-biased. We also ran a sensitivity analysis and also tried observing changes between original coloured images and an image with a filter put on it (sepia and grayscale).

<span style="color:#5DADE2;font-style:bold;font-size:120%">IMPACT</span>

We found out that the model, in some cases, was biased towards text present in the image (which was mostly Tokyo 2020). We also found in several cases, where the main focus of the image, the athletes were not the ones selected as the most salient in the image, instead, the saliency model was predicting either someone from the audience or billboards / advertisements as the most salient. This report was submitted to Twitter and we got a thanks from the Twitter team for highlighting this bias in their model.