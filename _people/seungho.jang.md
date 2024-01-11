---
layout: people
background: /assets/images/kaist.jpg
title: Seungho Jang (장승호)
excerpt: "Seungho Jang's website"
---

{%- assign person_id = "seungho.jang" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/seungho.jang.jpg" alt="{{ person.name }}">

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr/)**.

{% include person_contact.md person_id=person_id %}
{% include person_education.md person_id=person_id %}

#### Experiences

- Undergraduate Intern, Computer Architecture and Systems Lab, Kaist, June 2023 ~ October 2023 \
  (topic: Completely Fair Scheduler in Rust Operating System)
