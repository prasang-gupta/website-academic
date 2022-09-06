---
title: Automated PPT content editor
subtitle: <span style="font-size:80%;color:#5DADE2">[ PwC US ] </span><span style="font-size:80%"><a href="https://www.linkedin.com/in/millennium-bismay/" target="_blank">Millennium Bismay</a>, Prasang Gupta, <a href="https://www.linkedin.com/in/vishakhabansal91/" target="_blank">Vishakha Bansal</a>, <a href="https://www.linkedin.com/in/shazhoda/" target="_blank">Shaz Hoda</a></span>
summary: Built a solution that transforms a non-formatted PPT file to a formatted PwC-compliant file including several Editorial, Branding and Alignment modules using lxml open office format
tags:
- Automation
- Formatting
- Open Office XML (lxml)
- Machine Learning
- Firm Internal
- ML-DL

date: "2021-08-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Alignment on Powerpoint
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

<span style="font-style:bold;font-size:120%"><a class="mt-1">AIM</a></span>

The aim of this project was to generate a solution that would auto-format any PPT in PwC-compliant format. The changes included several editorial changes (word alternatives, punctuations) and branding changes (colors, formatting). It also included aligning any misaligned objects present in the PPT.

<span style="font-style:bold;font-size:120%"><a class="mt-1">DETAILS</a></span>

We decided to edit the underlying XML format of the presentation (using the open office lxml format) in addition to actually editing the PPT itself. We wrote code to parse the PPT in an editable format and then created a modular structure to work on different portions of the PPT. Some modules were rule-based, some were logic driven based on the requirements and some modules incorporated ML solutions developed for sub-problems wherever possible. Some of the modules built were:

| Module | Type | Function and Details |
|-|-|-|
| Word | Editorial | Performed changes on the word level. One was making them consistent in terms of American English / British English. Also included removing any risk words and replace jargons with better suited alternatives |
| Numbers | Editorial | Performed date parsing, currency conversions etc based on the format expected. Also changed numerical numbers to text wherever applicable |
| Punctuation | Editorial | Added and modified punctuation marks wherever applicable in a consistent format |
| Paragrapsh | Editorial | Identified any lengthy paragraphs or capitalisation issues in the presentation and gave suggestions to shorten it | 
| Font | Branding | Changed font sizes, styles and colors based on the location of the text (header, help box, content box etc) |
| Bullets | Branding | Formatted simple and nested bullets to follow a particular pattern and adjusted font size and bullet marker according to the context |
| Header and Footer | Branding | Adjusted header and footer in the master slide to be put on every slide in the document. Also, detected and accounted for repeated non-aligned headers and footers |
| Pictogram | Branding | Detected images present in the slides and checked whether they are approved pictograms or if they infringe any copyright claims |
| Colors | Branding | Changed the colors (font, background, pictograms) to be replaced with the nearest PwC-approved colors based off of a novel color matching technique |
| Animations | Branding | Detected and changed any animations in the presentation wherever applicable |

<span style="font-style:bold;font-size:120%"><a class="mt-1">IMPACT</a></span>

This solution built was deployed on an internal hosting service and was made available as a service. The total processing time for an average presentation was about 5 minutes with all the modules active. This brought down the time to manually review and format average presentations from 30 minutes to about 10 minutes. The solution was not perfect, but it helped ensure that most of the repetitive tasks are taken care of by the code and only final inspection with some modifications need to be done by the manual reviewers, saving thousands of manhours for the firm.