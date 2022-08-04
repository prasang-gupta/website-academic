---
title: Occupancy Detection
subtitle: 
summary: Built a solution for anonymised occupancy detection inside office space with LIDARs with features including social bubble breach detection and zone-based real-time occupancy counts and tracking
tags:
- IoT
- Occupancy Detection
- LIDAR

date: "2021-06-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Snapshot of the real-time occupancy detection dashboard
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

The client wanted to prepare for and ensure a safe transitioning of people from "Work from home" to Office space. They wanted to make sure that the facility should be used responsibly and at no time there should be breaches of the social distancing regulations.

* *OUR SOLUTION*

![Solution Architecture](architecture.png)

We prepared a solution that gave the client the ability to track and measure the occupancy and social distancing norms anonymously. We set up a LIDAR in the client office space attached with a hub to send the data to the cloud. Several calculations and checks were performed on the cloud and the final data was sent to the dashboard. The real time occupancy readings (both overall and zone-based) were also visualised by the dashboard.

* *VALUE GENERATED*

As a result of our solution, the client could monitor occupancy in real-time, track occupancy trends and monitor the hotspots in the office. This can further be used to optimise the office space usage.