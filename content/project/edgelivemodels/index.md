---
title: Implementation of live models on edge
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%">Prasang Gupta, <a href="https://www.linkedin.com/in/swayambodha-mohapatra-7a7a22110/" target="_blank">Swayambodha Mohapatra</a></span>
summary: Implemented and optimised multiple live models (eg. action recognition on something something dataset with over 200 classes) on edge devices (eg. Jetson TX2, Raspberry Pi)
tags:
- IoT
- Deep Learning
- Edge Devices
- AI on Edge
- NVIDIA Jetson TX2
- Raspberry Pi
- Live Action recognition
- Something Something Dataset
- Proof of Concept
- ML-DL

date: "2019-11-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Sample outputs of live model running on edge device
  focal_point: Smart

links:
- icon: 
  icon_pack: 
  name: Data
  url: https://20bn.com/datasets/something-something/v2#download
url_code: "https://github.com/zhoubolei/TRN-pytorch"
url_pdf: ""
url_slides: "https://drive.google.com/file/d/1vBp-ia0RgIUUHdnx4pCu8-1VqhJg7VRr/view?usp=sharing"
url_video: "https://drive.google.com/drive/folders/1M98mcE-RMoZTTL8sErfZzGLJXfdlOt5I?usp=sharing"

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

<span style="font-style:bold;font-size:120%"><a class="mt-1">AIM</a></span>

The aim of this project was two fold. The first aim was to implement an action recognition model and the second was to modify it to run on an edge device. For this, we chose the Pre-trained Temporal Relation Network Model. The dataset chosen for this was the 20BN-something-something Dataset V2. This dataset has over 100 classes of different object-human or object-object interactions.

![Jetson TX2](jetson.png)

<span style="font-style:bold;font-size:120%"><a class="mt-1">DETAILS</a></span>

The model was first implemented on a laptop with the webcam and then later extended onto the edge device, Jetson TX2. Prior to this, the TX2 was flashed and proper libraries were built from source to enable it to use its full potential (CUDA cores for rendering). We were successfully able to implement this on the board and were getting very respectable frame rates, somewhere around 10 fps. The performance of this model for several different scenarios can be seen in the videos link and a little detail about the implementation can be found in the slides.

Apart from this, we also implemented simple object detection models on Raspberry Pi on which we were getting around 1-2 fps.

<span style="font-style:bold;font-size:120%"><a class="mt-1">IMPACT</a></span>

These implementations paved the way for future projects that involved hosting models on smaller edge devices. These capabilities were built for the first time within the team.