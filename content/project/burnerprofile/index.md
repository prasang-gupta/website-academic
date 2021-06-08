---
title: Numerical Study of SiO2 Burner profiles
subtitle: '[Prasang Gupta](), [Sana Khanum](https://www.linkedin.com/in/sana-khanum-90625bb7), [Prof. Naveen Tiwari](https://www.iitk.ac.in/che/nt.htm), [Prof. V Shankar](https://home.iitk.ac.in/~vshankar), [Prof. Goutam Deo](https://www.iitk.ac.in/che/gd.htm)'
summary: Performed a numerical study of SiO2 burner profiles simulating a burner flame and calculating the flame temperature profile and species distribution in the flame.
tags:
- Chemical Engineering
- Burner profile
- Adiabatic Temperature Calculation
- MATLAB
- COMSOL
- ANSYS Chemkin
- ASPEN Plus

date: "2017-04-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: A representation of burner velocity profile by IndustrialHeating
  focal_point: Smart

links:
url_code: "https://drive.google.com/drive/folders/1NHEFnwDFngm7aZyDGDY1XU72YYlm4omK?usp=sharing"
url_pdf: "https://drive.google.com/file/d/1q6NYtHTPrX0eVvhN_bCvZf7pssjW8GyZ/view?usp=sharing"
url_slides: "https://drive.google.com/file/d/17DYshGPp9Yd_lsbKarPL1Vqit8i0WuUh/view?usp=sharing"
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
This was an Undergraduate project under Prof. Naveen Tiwari, Prof. V Shankar and Prof. Goutam Deo from January 2017 to March 2017. The aim of the study was to model an SiO2 burner with specific dimensions and study the temperature profiles of the burner. The project also included studiyng the distribution of different species present at different distances away from the flame.

To kick off the modelling, adiabatic flame temperature was calculated for a hydrogen-oxygen combustion process. The equilibrium analysis was done on ASPEN Plus package. To validate the results, the same value was cross-referenced with literature values. It was found to be in good agreement with that. Next, a 100% conversion analysis was done using the same suite. However, this time the same model was built using first principles on MATLAB and the results were compared. Again, there was a very good agreement with both of these values. Hence, we concluded that the modelling process done in the ASPEN Plus suite is correct.

Having validated our model, we started experimenting with different conditions for the same process. This included changing the temperature as well as adding Silicon Tetrachloride in the feed. Finally, a dependence between the hydrogen flow rate with the adiabatic temperature was established.

Next, we moved on to the kinetics of the problem. The overall reaction was broken down into several different intermediate reactions. Every one of these intermediate reactions have different kinetic parameters. All the possible intermediate reactions were written and validated with theroy and literature. Preliminary reaction kinetics were performed with an assumed value of burner diameter and were qualitatively checked with literature values.

Further, the original burner dimensions were added to the model and all the calculations were re-run for this. The mole fractions of the different species were studied at the end of the flame. This provided much better view into the temperature variation in the flame and the different reaction progress with the length of the flame. This gave us the minimum length of the flame to ensure that the reaction gets over and a maximum conversion of raw materials to products can be achieved with minimal waste.