---
layout: people
background: /assets/images/kaist.jpg
title: Taewoo Kim (김태우)
excerpt: "Taewoo Kim's website"
---

{%- assign person_id = "taewoo.kim" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/taewoo.kim.jpg" alt="{{ person.name }}">

I am a **Master's Student at [KAIST School of Computing](https://cs.kaist.ac.kr/)**.
I'm interested in the design of OSes and other concurrent systems.

{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Awards and Honors

- Summa Cum Laude (4.24/4.3), KAIST, 2024.