---
title: L2RPN Hackathon 2020 - Robustness Track
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%"><a href="https://www.linkedin.com/in/vishakhabansal91/" target="_blank">Vishakha Bansal</a>, Prasang Gupta</span>
summary: RL-based challenge to robustly maintain an electrical grid without disruptions against an adverse agent. <span style="color:#5DADE2;font-style:bold;font-size:120%">Achieved 28th rank in the hackathon</span>
tags:
- Power network
- Adverse agent
- Reinforcement Learning
- CodaLab
- Hackathon
- ML-DL

date: "2020-10-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Visualisation of a power grid
  focal_point: Smart

links:
- name: Competition Page
  url: https://competitions.codalab.org/competitions/25426#learn_the_details
url_code: "https://github.com/prasang-gupta/L2RPN-2020-robustness"
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

<span style="color:#58D68D">We achieved</span> <span style="color:#52BE80;font-style:bold;font-size:120%">28th rank</span> <span style="color:#58D68D">in the hackathon.</span>

<span style="color:#5DADE2;font-style:bold;font-size:120%">AIM</span>

The aim of L2RPN (Learning to Run a Power Network) 2020 hackathon - Robustness Track was to build a robust agent that would be keep delivering reliable electricity everywhere and also operate the grid safely when an agent takes unknown adversarial actions at regular intervals.

<span style="color:#5DADE2;font-style:bold;font-size:120%">DETAILS</span>

The dataset contained episodes spanning different adversarial actions taken by the agent. The agent could terminate any 1 of the 10 possible power lines (some of them being high voltage lines). Our agent was to be evaluated on how long it can provide reliable power to consumers without causing blackout. Once a blackout occurs, it is game over for that episode. The operation cost to be minimized included powerline losses, redispatch cost and blackout cost.

Every substation in the competition grid had a "double busbar layout". Hence, there was a choice of bus for making a connection from one of the bus to a grid object. Due to this and the medium sized grid used, the action space was of the order of 10^5 with the combinatorial action space reaching infinity.

Our approach was derived from a previous [public solution](https://github.com/ZM-Learn/L2RPN_WCCI_a_Solution) for this competition. THe idea was to reduce the action space and train 2 A3C models with different training parameters.

<span style="color:#5DADE2;font-style:bold;font-size:120%">IMPACT</span>

We managed to improve upon the baseline set and managed to achieve a score of 10.84, which was the 21st highest score on the leaderboard, gaining us 28th rank.