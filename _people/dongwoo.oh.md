---
layout: page
title: Dongwoo Oh (오동우)
excerpt: "Dongwoo Oh's website"
---

{%- assign person_id = "dongwoo.oh" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}


I am an **Undergraduate Student at [Department of Mathematical Sciences at KAIST](https://mathsci.kaist.ac.kr/home/)**.
I'm interested in various topics including but not limited to verification of
concurrent and distributed systems, tools for easier concurrent programming,
and type systems.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}


#### Publications

{% include publications.md author_id=person_id submitted=true %}

