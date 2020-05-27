---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Boogui"
summary: "Boogui is a software dedicated to viewing and processing gaze data recorded with EyeLink or SMI eye trackers."
authors: []
tags: [eyetracking]
categories: []
date: 2020-03-16T10:20:54+01:00

# Optional external URL for project (replaces project detail page).
#external_link: "https://github.com/jbourgin/Boogui"

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: "https://github.com/jbourgin/Boogui"
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# Attention, le lien SMI ne marche plus à cause du rachat. Plus de site officiel ?
slides: ""
---

Boogui (named so after the great [Boo](https://baldursgate.fandom.com/wiki/Boo), who was always keen to "go for the eyes") is a software dedicated to viewing and processing gaze data recorded with [EyeLink](https://www.sr-research.com/) or [SMI](https://www.smivision.com/) eye trackers.

![Screenshot](/img/boogui.png)

Boogui currently includes:
* Visualization of gaze data over time for each trial with target frames displayed
* A video view that plays back the trial with eye movements overlaid
* Filtering of SMI data based on fixation / saccade / blink parameters (e.g. duration). Compared to the default algorithm provided by SMI, it takes into account artifacts and allows to consider both dispersion and velocity for more accurate calculation of fixations.
* Output reports (.txt or .csv files) that can then be directly imported in statistical analysis packages such as Statistica or R for further processing.

Boogui currently implements experiments conducted during a thesis work conducted by Jessica Bourgin:
* Visual search
* Pro-saccade/anti-saccade
* Gaze-contingent
* Saccadic choice
