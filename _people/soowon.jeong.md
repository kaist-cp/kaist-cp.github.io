---
layout: page
title: Soowon Jeong (정수원)
excerpt: "Soowon Jeong's website"
---

{%- assign person_id = "soowon.jeong" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr)**. 
I am interested in programming language and formal verification. I joined [Concurrency and Parallelism Laboratory](https://cp.kaist.ac.kr) to study about formal verification.

{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Experiences

- Intern, Pilab, August, 2019 - December, 2019, March, 2020 - June, 2020.

  (topic: Programming language for developing smart contracts)
