---
layout: page
title: Chaeeun Hwang (황채은)
excerpt: "Chaeeun Hwang's website"
---

{%- assign person_id = "chaeeun.hwang" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr)**. 
I wanted to study computer systems more deeply through various languages, so I joined [Concurrency and Parallelism Laboratory](https://cp.kaist.ac.kr).

{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}
