---
layout: archive
title: "CV"
permalink: /
author_profile: true
redirect_from:
  - /resume
  - /cv
---

{% include base_path %}

Education
======
* Ph.D in Software Engineering, ECNU (expected)
* B.S. in Cyber Security, Xidian University, 2026

Work experience
======
* Fall 2024: Quality Engineer
  * AVIC FACRI
  * Duties includes: Updates and improvements to testing framework
  
Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
