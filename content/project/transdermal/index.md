---
title: Macroscopic model for Transdermal Drug Delivery
subtitle: '[Prasang Gupta](), [Kishore Gajula](https://www.linkedin.com/in/kishore-gajula-32746824/), [Rakesh Gupta](https://www.linkedin.com/in/rakesh-gupta-a49b4459/), [Beena Rai](https://www.linkedin.com/in/beena-rai-7a6a3713/)'
summary: Developed a macroscopic model of skin's upper layer (Stratum Corneum) to study transdermal drug delivery and effectiveness of electroporation on drug transfer.
tags:
- Chemical Engineering
- Transdermal Drug Delivery
- Electroporation
- Skin modelling
- OpenFOAM
- C++

date: "2017-07-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: A representation of transdermal drug delivery from [Oral Delivery of Insulin](https://www.sciencedirect.com/book/9781907568473/oral-delivery-of-insulin)
  focal_point: Smart

links:
- icon: 
  icon_pack: 
  name: Data
  url: https://drive.google.com/drive/folders/1XyvqHHwcZCAiGrD8JyacgnI5M_9dDGha?usp=sharing
url_code: ""
url_pdf: "https://drive.google.com/file/d/1kIQ7dooN_z5BepuAYVm9V-Kby_1gBYZv/view?usp=sharing"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
This project was part of my internship at TATA Research Design and Development Centre. The internship started May 2017 and ended July 2017. The objective of the project was to develop a macroscopic model of skin’s upper layer stratum corneum using OpenFoam, an open-source library. This library was chosen as this provided and open source FVM alternative to the licensed FEM solver, COMSOL. Apart from that, nobody in the firm had used it before, so it served as an exploration study into using this library. However, as I was able to finish the objective early, I also finished an extension of the project, which included studying the effects of electroporation on the drug transfer kinetics.

The first task was to get used to the OpenFOAM library which is completely CLI based. After getting a handle of the different methods and way of working, the first model was developed of the uppermost skin layer, Stratum Corneum using a parameterised brick and mortar structure. This model was then used to model a transdermal drug delivery by Fickian diffusion through the layer.

Fentanyl and Caffeine were chosen to be studied based on literature review and their scope of usage in transdermal delivery. The diffusion coefficients for these components were obtained from MD simulations. Running them through the developed model provided drug release profiles for both. These profiles were validated by experimental studies present in literature.

Since, there were a lot of files that needed to be modified to set up an OpenFOAM simulation, running iterations while maintaining correctness (not missing editing a file) was a steep task. Hence, I worked on automating the whole simulation process and file editing structure using C++ and Bash. This reduced simulation set up times drastically allowing me to run several iterations and complete the objective of my internship way before my internship end date.

As a result, I was able to extend the study to include the effects of electroporation on the drug delivery profiles. The new model developed with electroporation was again validated with experimental data and was found to be in good agreement. Also, the drug release significantly increased after using electroporation which was expected from the study.