---
layout: people
background: /assets/images/kaist.jpg
title: Minseong Jang (장민성)
excerpt: "Minseong Jang's website"
---

{%- assign person_id = "minseong.jang" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/minseong.jang.jpeg" alt="{{ person.name }}">

I am a **Master Student at KAIST [School of Computing](https://cs.kaist.ac.kr)** at [Concurrency and Parallelism Laboratory](https://cp.kaist.ac.kr).

I am currently working on [designing high-level hardware description language]({{ site.baseurl }}{% link _projects/fpga.md %})

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}

#### Publications

{% include publications.md author_id=person_id submitted=true %}

#### Experiences

- Software Engineer, Waddle Corporation, April, 2019 - January, 2021.
  
  (topic: Back-end development, R&D)
