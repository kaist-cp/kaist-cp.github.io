---
layout: page
title: Batzorig Zorigoo
excerpt: "Batzorig Zorigoo's website"
---

{%- assign person_id = "batzorig.zorigoo" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl}}/assets/batzorig.zorigoo.jpg" alt="{{ person.name }}">

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr)**. I
am currently interested in optimizating all kinds of systems and algorithms using 
concurrency and parallelism.


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Experiences

- Computer Vision Intern, Crazing Lab, June, 2019 - August, 2019.

  (topic: Approximating baseball rotational speed in real-time)

- Robotics Intern, Crazing Lab, December, 2018 - February, 2019.

  (topic: Driver for Camera Operating Robot (UR3e, Segway RMP, UMC-S3CA))
