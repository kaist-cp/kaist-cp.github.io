---
layout: people
background: /assets/images/kaist.jpg
title: Kisoo Kim (김기수)
excerpt: "Kisoo Kim's website"
---

{%- assign person_id = "kisoo.kim" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/kisoo.kim.jpeg" alt="{{ person.name }}">

I am an **Undergraduate Student in [KAIST Department of Mathematical Science](https://mathsci.kaist.ac.kr)** and **[KAIST School of Computing](https://cs.kaist.ac.kr)**.

Currently, I am interested in the formal verification by computer in practical applications, i.e. compilers or systems.
I am looking for learning how to design and verify concurrent and parallel systems by joining and working at **[Concurrency and Parallelism Laboratory](https://cp.kaist.ac.kr)**.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}
