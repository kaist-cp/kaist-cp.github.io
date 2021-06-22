---
layout: people
background: /assets/images/kaist.jpg
title: Jung In Rhee (이정인)
excerpt: "Jung In Rhee's website"
---

{%- assign person_id = "jungin.rhee" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

I am a **Undergraduate Student at KAIST [School of Computing](https://cs.kaist.ac.kr)**. I am interested in designing concurrent and parallel systems. Currently I am studying [Rust](https://www.rust-lang.org).


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}
