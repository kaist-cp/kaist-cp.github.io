---
layout: people
background: /assets/images/kaist.jpg
title: Janggun Lee (이장건)
excerpt: "Janggun Lee's website"
---

{%- assign person_id = "janggun.lee" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/janggun.lee.jpg" alt="{{ person.name }}">

I am a **Master Student at KAIST [School of Computing](https://cs.kaist.ac.kr)** at [Concurrency and Parallelism Laboratory](https://cp.kaist.ac.kr). 

My interest lies in formal verfication of real-world systems using [Coq](https://coq.inria.fr/).

Currently, I am researching on verification of concurrent data structures on weak memory.


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}
