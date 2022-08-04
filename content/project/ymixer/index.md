---
title: Numerical Investigation of Nanoparticle Precipitation in Y-Mixers
subtitle: '[Prasang Gupta](), [Swati Sahu](https://www.linkedin.com/in/sahuswati), [Prof. Nishith Verma](https://www.iitk.ac.in/che/nv.htm)'
summary: Performed a simulation study of nanoparticle precipitation in 2D and 3D Y-mixers solving the population balance equation. The study included fluid flow and tracer analysis using both C++ and palabos library.
tags:
- Chemical Engineering
- Population Balance
- Nanoparticle precipitation
- palabos
- C++

date: "2016-12-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Tracer analysis on y mixer
  focal_point: Smart

links:
- icon: 
  icon_pack: 
  name: Data
  url: https://drive.google.com/drive/folders/1e75PPb00gnr5FUiGXzsOgR0Llow2ITl8?usp=sharing
url_code: ""
url_pdf: "https://drive.google.com/file/d/1nLsYK2B26oFwA1dJ9sMEKtBOxs0G7tOB/view?usp=sharing"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

This was an Undergraduate project under Prof. Nishith Verma which went on from March 2016 to December 2016. Our aim was to perform an investigation into the particle densities obtained by mixing two fluids in a Y-shaped mixture.

As a first step, the y mixer model was generated in C++ in 2 and later 3 dimensions and simulations were run using the Lattice Boltzmann method. This resulted in fluid flow diagrams which were matched with experiments. After validating this model, tracer analysis was done on the outputs. This ensured us to capture the cross section and the mixing capabilities of the mixer. This was again validated from experiments.

Having a C++ lattice boltzmann model ready, we moved on to using the palabos library to include population balance equations in our simulation model. This included the new calculations as well as sped up the entire code by about 40%. Nucleation rates and growth rates for the different particles were provided based on experimental chemical reactions and the population density of the product was studied at different cross sections of the mixer representing varying mixer sizes.
