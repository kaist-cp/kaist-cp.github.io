---
layout: people
background: /assets/images/kaist.jpg
title: Jaeyong Sung (성재용)
excerpt: "Jaeyong Sung's website"
---

{%- assign person_id = "jaeyong.sung" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/jaeyong.sung.jpg" alt="{{ person.name }}">

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr)**.

I am interested in designing concurrent and parallel systems.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}
