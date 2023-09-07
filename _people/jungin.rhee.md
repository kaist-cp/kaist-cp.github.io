---
layout: people
background: /assets/images/kaist.jpg
title: Jung In Rhee (이정인)
excerpt: "Jung In Rhee's website"
---

{%- assign person_id = "jungin.rhee" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/jungin.rhee.jpg" alt="{{ person.name }}">

I am a **Master Student at KAIST [School of Computing](https://cs.kaist.ac.kr)** at [Concurrency and Parallelism Laboratory](https://cp.kaist.ac.kr).

I am currently working on [designing high-level hardware description language]({{ site.baseurl }}{% link _projects/fpga.md %})


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}
