---
layout: people
background: /assets/images/kaist.jpg
title: Gieun Jeong (정기은)
excerpt: "Gieun Jeong's website"
---

{%- assign person_id = "gieun.jeong" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/gieun.jeong.jpg" alt="{{ person.name }}">

I am an **Undergraduate Student in [Inha University Computer Science and Engineering](https://cse.inha.ac.kr/cse/index.do)**. I'm going to be a **Master Student at [Graduate School of AI Semiconductor](https://aisemi.kaist.ac.kr/)** and join CP lab in 2024 spring.

I am studying foundations about CP lab’s research topics. Especially, I am interested in the Shakeflow project.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}

#### Experiences

- Intern, Computer Architecture and Memory System Lab, Inha University, December 2022 ~ Present \
  (topic: Processing-in-Memory, AI accelerator)
