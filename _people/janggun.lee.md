---
layout: people
background: /assets/images/kaist.jpg
title: Janggun Lee (이장건)
excerpt: "Janggun Lee's website"
---

{%- assign person_id = "janggun.lee" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/janggun.lee.jpg" alt="{{ person.name }}">

I am a **Ph.D Student at KAIST [School of Computing](https://cs.kaist.ac.kr)** at [Concurrency and Parallelism Laboratory](https://www.fearless.systems).

My interest lies in formal verfication low-level concurrent data structures and systems.
I am especially interested in modular and automatic verification of them using separation logic such as [Iris](https://iris-project.org).


{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}

#### Publications

{% include publications.md author_id=person_id submitted=true %}
