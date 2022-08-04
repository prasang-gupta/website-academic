---
title: Fingervein Detection
subtitle: 
summary: Designed an end-to-end biometric system with user registration and verification as a replacement for fingerprint technology
tags:
- IoT
- Fingervein Detection
- Biometrics

date: "2020-10-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Jetson TX2 board
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
The aim of this project was to build out a fully functional proof of concept for the fingervein detection biometric system. This end-to-end system would include a frontend for new user registration, verification of user fingervein and deletion. We achieved this using a Fingervein device and a custom built secure backend database.

All the services were defined as part of an API which was hosted on a cloud platform. All the information transfer was done after using encryption. Furthermore, the frontend was built as a Google Chrome extension and integrated right into the browser for easy usage. This would ensure scalability and hassle free adoption.