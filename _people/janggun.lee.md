---
layout: page
title: Janggun Lee (이장건)
excerpt: "Janggun Lee's website"
---

{%- assign person_id = "janggun.lee" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}


I am a **Undergraduate Student at KAIST [department of Mathematical Sciences](https://mathsci.kaist.ac.kr) and [School of Computing](https://cs.kaist.ac.kr)**. To learn and research about formal verification of concurrent systems, I gladly joined the [Concurrency and Parallelism Laboratory](https://cp.kaist.ac.kr).


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}
