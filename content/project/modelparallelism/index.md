---
title: Model Parallelism for Inference at edge
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%"><a href="https://www.linkedin.com/in/venkat-will-not-give-up/" target="_blank">Venkata Koyya</a>, <a href="https://www.linkedin.com/in/siddhesh-zanj-2b934496/" target="_blank">Siddhesh Zanj</a>, Prasang Gupta</span>
summary: Implemented a solution that uses model parallelism for speeding up inference at the edge by distributing a single model across different devices
tags:
- Model Parallelism
- IoT
- Edge
- Deep Learning
- Proof of Concept
- ML-DL

date: "2021-11-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Channel Shuffle, an integral part of model parallelism
  focal_point: Smart

links:
- icon: 
  icon_pack: 
  name: Data
  url: https://www.kaggle.com/competitions/tiny-imagenet/data
url_code: "https://github.com/sysu-eda/Distributed-CNN-Inference"
url_pdf: "/project/modelparallelism/du2020.pdf"
url_slides: "https://docs.google.com/presentation/d/1P3X7MFR5m5Rq_b8-4cUGkwmrqdQlgOu9"
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

<span style="color:#5DADE2;font-style:bold;font-size:120%">AIM</span>

The aim of this project was to create a solution that can be used to train a model that can be split into multiple pieces and can be run in parallel on multiple separate devices.

<span style="color:#5DADE2;font-style:bold;font-size:120%">DETAILS</span>

![Solution Architecture](architecture.png)

The architecture used was the recently published DeCNN (Decoupled CNN) network. The authors had used GConv with Channel Shuffle and added other network and OS level modifications to improve the performance of the decoupled architecture. For initial testing, we only focused on Scheme 1 and ignored other optimisations to establish a baseline.

We used the tiny imagenet dataset and Resnet-34 model for testing and comparing the standard CNN results with DeCNN. We compared based on the performance (accuracy metrics) and the time taken to run inference on a fixed batch of data. It was found that there was a performance decrease by using DeCNN as some of the information is lost while doing channel shuffling. To counter that, we used 1.5x kernels as in the standard CNN to keep the performance comparable. Even while using just the Scheme 1 mentioned above, we got about 15% bump up in inference speeds with just 2 devices. We expect that this gap would increase with larger models and with more number of parallel devices.

<span style="color:#5DADE2;font-style:bold;font-size:120%">IMPACT</span>

The solution developed can be used to train models specifically for running on smaller edge devices. This is especially helpful as no single device can hold the full model in memory at the edge due to size and compute limitations and this would help in running bigger and better models at the edge with no added requirement of a heavy compute engine deployment.