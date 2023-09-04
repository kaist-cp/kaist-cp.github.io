---
layout: people
background: /assets/images/kaist.jpg
title: Woojin Lee (이우진)
excerpt: "Woojin Lee's website"
---

{%- assign person_id = "woojin.lee" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/woojin.lee.jpg" alt="{{ person.name }}">

I am an **Graduate Student at [Graduate School of AI Semiconductor](https://aisemi.kaist.ac.kr/)**.
I am interested in, but not limited to Sys for ML, Harmonizing HW and SW, AI Accelerator.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}

#### Experiences
- Internship, [KC-ML2](https://www.kc-ml2.com/), Sep.2020 - Feb.2021.
  
  (topic: Exploring ML HWs using TVM and Xilinx PYNQ board)
