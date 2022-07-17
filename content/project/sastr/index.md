---
title: Semi-Autonomous Surveillance and Tranportation Robot
subtitle: <span style="font-size:80%;color:#5DADE2">[ IIT Kanpur ] </span><span style="font-size:80%"><a href="https://www.linkedin.com/in/dgangwar20/" target="_blank">Deepak Gangwar</a>, <a href="https://www.linkedin.com/in/shibhansh-dohare/" target="_blank">Shibhansh Dohare</a>, <a href="https://www.linkedin.com/in/vaibhav-bhagat-380978a3/" target="_blank">Vaibhav Bhagat</a>, <a href="https://www.linkedin.com/in/snehilverma41/" target="_blank">Snehil Verma</a>, Prasang Gupta</span>
summary: Developed an all-terrain vehicle capable of automatic navigation and surveillance using Embedded systems and Google Maps API.
tags:
- Robotics
- CAD Design
- Localisation and Surveillance

date: "2015-07-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: CAD Design of the Robot
  focal_point: Smart

links:
url_code: ""
url_pdf: ""
url_slides: "https://drive.google.com/file/d/1LaRUTQrvF-ha5m1mJMEOqJEySMiPx19s/view?usp=sharing"
url_video: "https://www.youtube.com/watch?v=oLeQH6g9hCo"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

<span style="color:#5DADE2;font-style:bold;font-size:120%">AIM</span>

This project was done as a part of the summer project offering from Robotics Club, IIT Kanpur. The aim of this project was to build an all-terrain robot capable of autonomous navigation and provide surveillance in remote areas.

<span style="color:#5DADE2;font-style:bold;font-size:120%">DETAILS</span>

We modelled the robot on Solidworks and machined it using aluminium and CNC machines. For navigation, we integrated the IMU sensor with the GPS anc coupled them together iwth a Kalman filter. Also, we imported Google Maps API for setting the route to be travelled and later converted the route into different waypoints to be followed. This waypoint file was uploaded to the robot's APM (mission planner).