---
title: Cross-country Asset Tracking
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%">Prasang Gupta, <a href="https://www.linkedin.com/in/antoinetteyoung/" target="_blank">Antoinette Young</a>, <a href="https://www.linkedin.com/in/vijay-ujjain/" target="_blank">Vijay Ujjain</a></span>
summary: Tracked cargo shipment using cost-effective sensors along its cross-country journey from factory to distribution center ascertaining possible locations of damage for effective preventive steps
tags:
- IoT
- Asset Tracking
- Cost-effective sensors
- Logistics
- Low Code AEP
- Client Delivery

date: "2020-03-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Snapshot of the tracking dashboard given to the client
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

<span style="font-style:bold;font-size:120%"><a class="mt-1">PROBLEM</a></span>

The client were facing problems with cargo damage while in transit which were resulting in huge losses for them. Also, since the transit included multiple contractors responsible for different stretches of the overall route, and nobody was taking responsibility for the damages, they were at a loss and had no idea how to rectify this.

<span style="font-style:bold;font-size:120%"><a class="mt-1">SOLUTION</a></span>

{{< figure src="architecture.png" caption="Solution Architecture" theme="light">}}

We created an end-to-end asset tracking system for the client. The clients were given low-cost devices housing different sensors to include them with their shipments. These devices were very small (about 2cm x 2cm x 1cm) and were tested for harsh weather. Also, these devices were equipped with a battery, a GPS and cellular communication technology along with the accelerometer, humidity and temperature sensors. These were configured to be used as one time use devices to save on device recovery costs / logistics. They were configured to report information all along the journey and last the whole shipment time without the need of a recharge.

Thresholding was done on the accelerometer sensor housed in the device to store high impacts faced by it, which would directly correlate with the damage faced the equipment. These raw accelerometer values were then configured to be sent to the cloud managed by the manufacturer. This data was then available to be used using simple API requests.

The raw data collection and conversion to impact system was built on an application enablement platform. This resulted in quick prototyping and testing of the proof of concept. The processed data was then sent to a live dahsboard which was shared with the client for their perusal. This dashboard offered several important metrics such as the last known location, temperature and battery of the device. It also showed the impact values versus timestamp which were recorded by the device.

<span style="font-style:bold;font-size:120%"><a class="mt-1">IMPACT</a></span>

From using this solution, we were able to ascertain different impact values faced by the device during different portions of the journey. This helped the client to visualise and piece together possible regions where the shipment was getting damaged. Our analysis found that most of the impacts registered by the device were when the device was travelling from the factory to the ports, which was contrary to the earlier belief of the client that most of the damage was being caused during the ship route. This allowed the client to focus on that section and helped them save a lot of revenue spent on replacing damaged products as well as save the reputation of the company.