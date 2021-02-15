---
layout: page
title: Haroon Ahmed
excerpt: "Haroon Ahmed's website"
---

{%- assign person_id = "haroon.ahmed" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl}}/assets/haroon.ahmed.jpeg" alt="{{ person.name }}">

I am a **PhD Student at [Concurrency and Parallelism Laboratory]({{ site.url }}), [KAIST School of Computing](https://cs.kaist.ac.kr)**. I am working with  [Prof. Jeehoon Kang]({{ site.baseurl }}{% include person_url.md person_id="jeehoon.kang" %}) on hardware accelerators. 

#### Resaerch Interest
- Computer architecture 
- FPGA design and verification
- AI hardware accelerators
- Dynamically reconfigurable processors


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}

#### Experiences

- Hardware Engineer, Sahil Semiconductors, December, 2020 - March, 2021.

  (topic: ASIC design and verification)

- FPGA Design Engineer, Simmir Vision (Shanghai) CO., Ltd., January, 2019 - July,   2021.

  (topic: FPGA Enabled-AI Cameras)
  
#### Publications

{% include publications.md author_id=person_id submitted=true %}

#### Awards and Honors

- Fully-funded graduate fellowship,China. (2015-2017)
- KAIST graduate scholarship.(2021-present)
