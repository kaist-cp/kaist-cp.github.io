---
layout: page
title: Seoyun Son (손서윤)
excerpt: "Seoyun Son's website"
---

{%- assign person_id = "seoyun.son" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr)**. 
I wanted to study more about the computer system field, so I joined [Concurrency and Parallelism Laboratory](https://cp.kaist.ac.kr).

{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Experiences

- Intern, STS Lab(Kaist Civil & Environmental Engineering), March, 2017 - June, 2019

  (topic: Programming traffic simulations)