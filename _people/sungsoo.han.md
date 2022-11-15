---
layout: people
background: /assets/images/kaist.jpg
title: Sungsoo Han (한성수)
excerpt: "Sungsoo Han's website"
---

{%- assign person_id = "sungsoo.han" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/sungsoo.han.jpg" alt="{{ person.name }}">

I am an **Masters Student at Concurrency and Parallelism Laboratory, [KAIST School of Computing](https://cs.kaist.ac.kr)**. I joined this lab because it deeply matched my interests in software parallelism and language theory.


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Publications

{% include publications.md author_id=person_id submitted=true %}

#### Experiences

- Intern, 파인디지털, September, 2018 - February, 2019

  (topic: Navigation assistance using deep learning)
