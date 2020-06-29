---
layout: page
title: Jeong Woon Choi (최정운)
excerpt: "Jeong Woon Choi's website"
---

{%- assign person_id = "jeongwoon.choi" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr)**.


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}

{% include person_experience.md person_id=person_id %}