---
title: Distributed Edge Compute
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%">Prasang Gupta, <a href="https://www.linkedin.com/in/zhi-kun-steven-yang/" target="_blank">Zhi Yang</a>, <a href="https://www.linkedin.com/in/vijay-ujjain/" target="_blank">Vijay Ujjain</a></span>
summary: Built a system capable of distributing compute across different devices on edge using load balancing and micro kubernetes engine
tags:
- IoT
- Distributed Compute
- Compute at Edge
- Proof of Concept
- ML-DL

date: "2021-06-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Snapshot of the resource tracking dashboard
  focal_point: Smart

links:
url_code: "https://github.com/prasang-gupta/distributed-edge"
url_pdf: ""
url_slides: "https://docs.google.com/presentation/d/1KF2YjWAfGonhgAnZ6mfZNZ9JJdcLJY0-"
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

<span style="font-style:bold;font-size:120%"><a class="mt-1">AIM</a></span>

The aim of this study was to build a system to distribute compute load across different resources present on the edge. It also involved testing the built system with a dummy exercise and find out the robustness of the system and any additional points that might need to be taken care of before actually attempting a client project in this domain.

<span style="font-style:bold;font-size:120%"><a class="mt-1">DETAILS</a></span>

{{< figure src="architecture.png" caption="Solution Architecture" theme="light" >}}

We built out a system for distributed edge compute using microk8s, a micro kubernetes engine. We paired it with metalb, a load balancer and dashboarding, resource tracking and reporting tools like grafana and prometheus. To simulate an edge environment, a local ensemble of devices was created and connected together on the same network. A total of 3 devices were included in the network including a raspbery pi, a windows laptop and an edge compute appliance. For testing out the pipeline, we ran a simple object detection model on all the devices using tensorflow serving.

While testing, we also came across several limitations of the architecture. The first is that the compute power was very skewed within the networks (x86 devices were orders of magnitude faster than ARM). This lead to bottlenecking at times even with the load balancer. We also realised that running a full object detection model on small devices was not a great idea due to the compute and memory limitations of each device.

<span style="font-style:bold;font-size:120%"><a class="mt-1">IMPACT</a></span>

The system built was a demonstration that multiple unused devices can be pooled together at the edge to increase the overall compute capabilities, reducing the lag of transferring data to and from the cloud. Apart from reducing latency, it also helps in keeping the data secure as everything is happening locally. This also ensures that no single edge device is overutilised hampering the pipeline.