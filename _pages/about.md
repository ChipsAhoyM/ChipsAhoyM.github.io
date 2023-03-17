---
layout: about
title: About
permalink: /
subtitle: 

profile:
  align: right
  image: avatar.jpeg
  image_circular: false # crops the image to make it circular
  address: # empty 
  institution: PhD. Student, CS@PKU

news: false  # includes a list of news items
selected_papers: true # includes a list of papers marked as "selected={true}"
exp: true
social: true  # includes social icons at the bottom of the page
---

I am a second year Ph.D. student in the School of Computer Science, Peking University, advised by Prof. Boxin Shi at [Camera Intelligence Lab](https://ci.idm.pku.edu.cn). My current research area is Computational Photography and I mainly focus on neuromorphic cameras (e.g. DVS, Prophesee, Vidar). I hope to combine neuromorphic cameras with deep learning to build the next generation of camera systems through super-human visual sensing and computing.

I obtained my B.S. in Computer Science from the School of EECS as well as my B.H. in History from the Department of History at Peking University in 2021. During my undergraduate studies, I mainly worked on low-quality image enhancement guided by event cameras. And I am also interested in contemporary world history, especially the history of science and technology.

## Publications
<div class="publications">
{% for y in page.publication_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>