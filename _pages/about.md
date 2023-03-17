---
layout: about
title: about
permalink: /
description: PhD Candidate | Member of <a href="http://ci.idm.pku.edu.cn/" target="\_blank">Camera Intelligence Lab</a> | Computational Photography

profile:
  align: right
  image: avatar.jpeg
  address:

publication: true  # includes a list of papers
publication_years: [2023, 2022, 2021, 2020]  # to show the papers in these years
social: true  # includes social icons at the bottom of the page
---

## Education
I am currently pursuing a Ph.D. with Prof. Boxin Shi at Camera Intelligence Lab, School of Computer Science, PKU. My current research interest lies in Computational Photography and mainly works on Neuromorphic Cameras (e.g. DVS, Prophesee, Vidar). I am also interested in photography and world history.


<br>
<br>

## Publications
<div class="publications">
{% for y in page.publication_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>
