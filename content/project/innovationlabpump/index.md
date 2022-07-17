---
title: Centrifugal Pump Characteristics
subtitle: <span style="font-size:80%;color:#5DADE2">[ IIT Kanpur ] </span><span style="font-size:80%">Prasang Gupta, <a href="https://www.linkedin.com/in/prashant-singhla-79471199/" target="_blank">Prashant Singhla</a>, <a href="https://www.iitk.ac.in/che/at.htm" target="_blank">Prof. Anurag Tripathi</a></span>
summary: Studied the control characteristics of the centrifugal pump system. Derived the transfer function for flow rate and discharge pressure from the response of a step change in RPM and verified the same by further experimentation. Also, calculated the optimum RPM operation point for the Pump setup.
tags:
- Chemical Engineering
- Controls
- Transfer Function
- Centrifugal Pump characteristics

date: "2016-04-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Prediction of transfer function for centrifugal pump setup
  focal_point: Smart

links:
url_code: ""
url_pdf: ""
url_slides: "https://drive.google.com/file/d/1HViDidtvcW7iAUPe8t64vw9HnoOkGG9V/view?usp=sharing"
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

<span style="color:#5DADE2;font-style:bold;font-size:120%">AIM</span>

This was a part of the Unit Operations Lab course. The aim of this project was to innovate and go above and beyond the standard lab experiments with the same equipment. We were assigned the centrifugal pump setup which is originally used to study the effect of series and parallel setup of pumps on the discharge pressure and flow rate. We however decided to perform a very different study using the same equipment.

<span style="color:#5DADE2;font-style:bold;font-size:120%">DETAILS</span>

During our experiments, we noticed that there was a measurable gap between turning up the RPM of the motor and actually observing differences in the flow rate. This lead us to believe that there is some sort of a lag in play between the inputs and outputs. To model this lag, we assumed first order dynamics for simplicity and calculated the transfer function of the pump ny oberving the time difference it takes to reach equilibrium after giving the input. We later tested this obtained transfer function by further experimenting with the setup.

To ensure utmost accuracy in our calculation, we used high FPS cameras to record readings when we were giving a small step change as an input to the motor (change of RPM). We also performed an opimisation study for an optimum RPM for the motor for best energy efficiency.