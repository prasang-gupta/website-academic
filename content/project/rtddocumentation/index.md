---
title: Read-The-Docs Documentation Templatisation
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%"><a href="https://www.linkedin.com/in/bibhashm/" target="_blank">Bibhash Mitra</a>, Prasang Gupta, <a href="https://www.linkedin.com/in/zoraxl/" target="_blank">Zora Li</a>, <a href="https://www.linkedin.com/in/shinan-zhang-85264221/" target="_blank">Shinan Zhang</a></span>
summary: Explored sphinx and created a solution to automatically generate github-hosted documentation under 10 mins in RTD format
tags:
- Read The Docs
- Documentation
- Toolkit
- Automation
- Firm Internal

date: "2021-12-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Features of the templatised documentation
  focal_point: Smart

links:
url_code: "https://github.com/prasang-gupta/rtd-autodoc"
url_pdf: "/project/rtddocumentation/howtodocumentinrtd.pdf"
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

The aim of this project was to create a solution that would auto-create documentation given a code repository with docstrings. The main focus of this solution was be to allow generating quick documentation that can be hosted on Github pages for making it easier to re-use codebases because of a standardised documentation format.

<span style="font-style:bold;font-size:120%"><a class="mt-1">DETAILS</a></span>

We created a documentation template and chose RTD (Read The Docs) as standard formatting because of its popularity among open source tools. We built 2 methods within the solution, first focused on generating and hosting documentation quickly (under 10 minutes) and the second focused on learning the nitty-gritties of how Sphinx works and providing much more room for modifications and personalisation. This system can also be used to generate documentation in PDF format using latex.

<span style="font-style:bold;font-size:120%"><a class="mt-1">IMPACT</a></span>

The solution was used widely across different teams and it allowed easy re-use of code. It also cultivated a good culture of writing docstrings in functions and classes across the whole team.