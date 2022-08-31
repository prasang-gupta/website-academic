---
title: Worlds.io
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%">Prasang Gupta, <a href="https://www.linkedin.com/in/antoinetteyoung/" target="_blank">Antoinette Young</a>, <a href="https://www.linkedin.com/in/sindy-yixin-ma/" target="_blank">Sindy Ma</a></span>
summary: 
tags:
- IoT
- Worlds.io
- Digital Twin
- Simulation Modelling
- Deep Learning
- Proof of Concept
- ML-DL

date: "2021-07-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: New York City's Bryant Park used in the case study
  focal_point: Smart

links:
url_code: ""
url_pdf: ""
url_slides: ""
url_video: "https://drive.google.com/file/d/198q-E9mD_rMr6DEBi5jX4Uuzc5sC17Ep"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

<span style="font-style:bold;font-size:120%"><a class="mt-1">AIM</a></span>

The aim of this study was to test out some of the features offered by Worlds.io and create a generalised digital twin solution that can be leveraged in future projects. This would include generating a digital replication of their current environment and answer some of the questions based off of that with some additional analysis to allow clients to make better oeprational and strategic decisions.

<span style="font-style:bold;font-size:120%"><a class="mt-1">DETAILS</a></span>

![Solution Architecture](animation.gif)

We took the live footage provided by the vendor in New York City's Bryant Park as a case study. A YOLO model was put on the raw camera footage to capture some common objects like people, bins, animals (pets) etc. This was then converted into a streaming data format and sent to cloud with approximate latitude and longitude values as provided by the vendor based on the camera's location and field of view. These lat-lon values were then converted into cartesian coordinates, effectively treating Bryant park in a 2D plane for getting the data ready for digital twin studies. We also created a few zones and mapped the coordinates accordingly.

The conversion to cartesian coordinates helped us to map the pedestrian movement patterns in the field of view. Additionally, we also extracted other information to answer questions like:

- How many people are passing through our zones in the park?
- How long are people generally in the park for?
- How many people are sitting in the park?
- How many people are walking babies/strollers?
- How many tourists/suitcases ?
- Are people riding bikes in the park?
- How many deliveries with carts are made?
- How many people are walking pets in the park?
- How many people per hour, walking speed, which way are they going, 
- What % of people are stopping?

<span style="font-style:bold;font-size:120%"><a class="mt-1">IMPACT</a></span>

We were able to run analytics on the video feed and the derived variables. Also, we were able to generate a digital twin using the converted coordinates. This helped us build capability for any future projects that might entail the use of these technologies.