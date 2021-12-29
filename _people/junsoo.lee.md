---
layout: people
background: /assets/images/kaist.jpg
title: Junsoo Lee (이준수)
excerpt: "Junsoo Lee's website"
---

{%- assign person_id = "junsoo.lee" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/junsoo.lee.jpg" alt="{{ person.name }}">

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr)**.
I am interested in designing concurrent and parallel systems.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}

#### Experiences

- Server Software Engineer, Devsisters Corporation, July, 2019 - August, 2021.
  
  (topic: game server)
