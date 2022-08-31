---
title: Concept Drift Detection with Chatbots
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%"><a href="https://www.linkedin.com/in/siddhesh-zanj-2b934496/" target="_blank">Siddhesh Zanj</a>, Prasang Gupta, <a href="https://www.linkedin.com/in/vishakhabansal91/" target="_blank">Vishakha Bansal</a>, <a href="https://www.linkedin.com/in/shantanu-dev/" target="_blank">Shantanu Dev</a></span>
summary: Built a scikit-learn-like toolkit with capabilities to detect concept drift in image, text or audio data using an array of drift detection methods for monitoring and extending the life of production models
tags:
- Concept Drift
- Concept Evolution
- Toolkit
- Data Drift
- Model Drift
- Deep Learning
- Firm Internal
- ML-DL

date: "2021-07-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Simple representation of concept drift sources
  focal_point: Smart

links:
- icon: 
  icon_pack: 
  name: Data
  url: https://docs.google.com/document/d/1ctNvL2enWHDIKax_mO6UC0pWPiMCScdlkWz35M-0J1g
url_code: ""
url_pdf: ""
url_slides: "https://docs.google.com/presentation/d/1Olk1hrIFyQIJ7Iu1_rjjuyH-klsYL5yZ"
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

<span style="font-style:bold;font-size:120%"><a class="mt-1">AIM</a></span>

The aim of this project was to create a drift detection toolkit that can be easily used to detect drift in any type of data (image, audio or text) using a multitude of different drift detection methods to suit every problem under the sun. We also tested this toolkit's ease of use by several case studies of different mock data types and also by integrating this with a chatbot built using RASA architecture to generate a novel drift-aware monitored chatbot.

<span style="font-style:bold;font-size:120%"><a class="mt-1">DETAILS</a></span>

The drift detection toolkit was built using several different drift detection methods like :

| Drift Detection Type | Drift Detection Methods |
|-|-|
| Data distribution based methods | - Kolmogorov-Smirnov (KS) test<br>- Maximum Mean Discrepancy (MMD) test<br>- Least-Squares Density Difference (LSDD) test<br>- KMeans and Chi Square Test<br>- Equal Intensity KMeans (EIKMeans) and Chi Square Test |
| Drift magnitude based methods | - Relative drift using Jensen–Shannon (JS) Divergence |
| Uncertainty based methods | - Uncertainty Classifier |
| Error rate based methods | - Fisher’s Test<br>- Statistical Test of Equal Proportions (STEPD) |

We implemented these methods and verified that these methods are functioning properly using curated open-source datasets. After verifying all these methods for different types of data (text, audio and images), we implemented an integrated architecture with a chatbot built using RASA framework.

{{< figure src="architecture.png" caption="RASA process flow" theme="light">}}

The process flow diagram shows the working of the integrated system. We implemented several novel methods that ensured our solution remained as general as possible and it does not hamper the whole process in any way whatsoever. Additionally, in case drift is detected, we also made a training pipeline that would incorporate the changes in the model weights without having any model downtime. 

<span style="font-style:bold;font-size:120%"><a class="mt-1">IMPACT</a></span>

The solution developed can be implemented with most of the chatbots that are currently in production. Implementing our system would ensure that the model does not lose intent quickly, and if it does, then proper notifications are being provided to the user based on the drift detection systems in place. It would also provide the developer with all the data that is needed to troubleshoot any issues and if needed, retrain the model to counter the drift without experiencing any downtimes.