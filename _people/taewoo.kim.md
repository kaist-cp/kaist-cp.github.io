---
layout: people
background: /assets/images/kaist.jpg
title: Taewoo Kim (김태우)
excerpt: "Taewoo Kim's website"
---

{%- assign person_id = "taewoo.kim" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/taewoo.kim.jpg" alt="{{ person.name }}">

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr/)**.
I'm interested in the design and verification of OSes or other concurrent systems, especially using **[Rust](https://www.rust-lang.org/)**.

{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}
