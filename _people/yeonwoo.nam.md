---
layout: page
title: Yeonwoo Nam (남연우)
excerpt: "Yeonwoo Nam's website"
---

{%- assign person_id = "yeonwoo.nam" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}


I am a **Undergraduate Student at KAIST [department of Mathematical Sciences](https://mathsci.kaist.ac.kr) and [School of Computing](https://cs.kaist.ac.kr)**. I am interested in formal verification of concurrent systems.


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}
