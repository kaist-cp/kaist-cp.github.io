---
layout: people
background: /assets/images/kaist.jpg
title: Yeji Han (한예지)
excerpt: "Yeji Han's website"
---

{%- assign person_id = "yeji.han" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/yeji.han.jpeg" alt="{{ person.name }}">

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr)**.
I am interested in developing system programs in Rust.

I am currently working on projects for [persistent memory]({{ site.baseurl }}{% link _projects/pmem.md %}).

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}

#### Experiences

- Software Engineer, Lucentblock, July, 2020 - July, 2022.
  
  (topic: Back-end development)
