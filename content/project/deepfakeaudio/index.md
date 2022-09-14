---
title: Zero-Shot Deepfake Audio Generation
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%"><a href="https://www.linkedin.com/in/anudeepimmidisetty/" target="_blank">Anudeep Immidisetty</a>, <a href="https://www.linkedin.com/in/ameliabauer/" target="_blank">Amelia Bauer</a>, Prasang Gupta</span>
summary: Explored and created a web-hosted demo for a zero-shot deepfake audio generation model to generate audio from text using embeddings of short reference audio clips
tags:
- Zero-Shot
- Deepfake
- Deep Learning
- Audio Generation
- Text to Speech
- Demo
- Proof of Concept
- ML-DL

date: "2022-04-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: A representation of YourTTS model architecture used in the study
  focal_point: Smart

links:
- icon: 
  icon_pack: 
  name: Data
  url: https://docs.google.com/document/d/1ctgXGIDsY2hW3tjqoTyvNBJo4-suiX0X-hCRrKOPlWY
url_code: ""
url_pdf: "https://arxiv.org/pdf/2112.02418.pdf"
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

<span style="font-style:bold;font-size:120%"><a class="mt-1">AIM</a></span>

The aim of this project was to create a demo for generating speech from text in the voice of the user given the least amount of sample possible.

<span style="font-style:bold;font-size:120%"><a class="mt-1">DETAILS</a></span>

As the aim of this study was to create a demo, we chose to go ahead with Zero-Shot model as it takes practically no time to train and can start giving good results even with very little amount of sample data. The tradeoff with accuracy was accepted in favour of time. We tested different models, the most popular being YourTTS, SCGlowTTS and SV2TTS. On the basis of qualitative assessment on the representative test dataset, which included both male and female audio samples in 3 different accents (American, British and Indian), YourTTS model was selected as the clear winner.

After finalising the model, this was tested further for robustness and a minimum sample audio time was estimated based off of these tests and it came out to be 1 minute for getting decent results in most cases. We then deployed this solution on an internal hosting site and created an interactive demo using our developed model as the backend. A representative set of 10 small sentences were obtained which contain as many different phonetics as possible and then a feature was added to record the user speak these sentences.

<span style="font-style:bold;font-size:120%"><a class="mt-1">IMPACT</a></span>

After running these samples through the model, which takes about a minute, the user would be able to hear their deepfake speaking 5 different sentences that were not a part of the representative set in their voice. This rounded off a user-friendly demo that can be used for GTM strategies.