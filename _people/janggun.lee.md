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

My interest lies in formal verfication low-level concurrent data structures and systems.
I am especially interested in modular and automatic verification of them using separation logic such as [Iris](https://iris-project.org).

Currently, I am researching on improving the automation of [Diaframe](https://gitlab.mpi-sws.org/iris/diaframe), an automation tool for Iris.
I wish to improve its usability in aiding the proof of more complex data sturctures and systems, scaling up to thousands of lines of proof code.

I am also interested in designing specifications for weak memory data sturctures, especially for ones that does not have a clear sequential specification.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}

#### Publications

{% include publications.md author_id=person_id submitted=true %}
