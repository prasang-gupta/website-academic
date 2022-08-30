---
title: Intelligent Systematic Investment Agent
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%">Prasang Gupta, <a href="https://www.linkedin.com/in/shazhoda/" target="_blank">Shaz Hoda</a></span>
summary: Explored an ensemble of deep learning and evolutionary strategies as an RL alternative in the context of an investment problem
tags:
- Investment
- ETF Trading
- Reinforcement Learning
- Evolutionary Strategies
- Genetic Algorithm
- Deep Learning
- Firm Internal
- ML-DL

date: "2021-10-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Investment stats by GADLE algorithm
  focal_point: Smart

links:
- name: Publication
  url: publication/rlisia
- name: Data
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

<span style="color:#5DADE2;font-style:bold;font-size:120%">AIM</span>

The aim of this project was to explore Evolutionary strategies as an alternative to the classicaly used Reinforcement learning techniques to solve the ETF trading investment problem.

<span style="color:#5DADE2;font-style:bold;font-size:120%">DETAILS</span>

Historically, autonomous agents for trading and investment are generally built using one of the many reinforcement learning techniques. These include the SOTA Actor-critic algorithms as well as simpler DQN based algorithms. The problem with these is that an environment needs to be setup for training them and the learning curve for these algorithms is a bit steep for someone inexperienced in the field of Reinforcement Learning.

We demonstrated that using Evolutionary strategies to solve episodic problems (which is getting daily purchase actions for a month in the current problem) can be a much easier and robust method. We also coupled this with a simple Neural network model to learn the patterns that are being revealed in the outputs of the ES runs. This broke down the problem into 2 mutually exclusive parts, which is much easier to understand and code.

We compared both qualitative and quantitative metrics for our ensemble algorithm we call `GADLE` with 2 traditional RL-based solutions, Actor-critic and DQN. Qualitatively, we compared the ease of writing of code and ease of understanding. Quantitatively, we ran different experiments centered around performance, sensitivity and consistency of the solutions.

<span style="color:#5DADE2;font-style:bold;font-size:120%">IMPACT</span>

The proposed GADLE algorithm performs at par with the Actor-critic algorithm. However, it crushes the competition in terms of consistency and sensitivity. To put things in perspective, following are the tables summarising results of the sensitivity and the consistency experiments.

![Sensitivity comparison](sensitivity.png)

![Consistency comparison](consistency.png)