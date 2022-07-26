---
layout: people
background: /assets/images/kaist.jpg
title: Youngseok Choi (최영석)
excerpt: "Youngseok Choi's website"
---

{%- assign person_id = "youngseok.choi" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/youngseok.choi.jpg" alt="{{ person.name }}">

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr) and [Department of Mathematical Sciences](https://mathsci.kaist.ac.kr)**.
Currently, I am studying and working on formal verification.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}
