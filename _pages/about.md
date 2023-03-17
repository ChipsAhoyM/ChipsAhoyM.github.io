---
layout: about
title: About
permalink: /
subtitle: 

profile:
  align: right
  image: avatar.jpeg
  image_circular: false # crops the image to make it circular
  address: 

news: false  # includes a list of news items
publication: true
publication_years: [2023, 2022, 2021, 2020]
# selected_papers: true # includes a list of papers marked as "selected={true}"
exp: true
social: true  # includes social icons at the bottom of the page
---

I am currently pursuing a Ph.D. with Prof. Boxin Shi at Camera Intelligence Lab, School of Computer Science, PKU. My current research interest lies in Computational Photography and mainly works on Neuromorphic Cameras (e.g. DVS, Prophesee, Vidar). I am also interested in photography and world history.

## Publications
<div class="publications">
{% for y in page.publication_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>
