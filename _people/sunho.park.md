---
layout: people
background: /assets/images/kaist.jpg
title: Sunho Park (박선호)
excerpt: "Sunho Park's website"
---

{%- assign person_id = "sunho.park" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/sunho.park.jpg" alt="{{ person.name }}">

I am a **Master's Student at [KAIST School of Computing](https://cs.kaist.ac.kr)**.
I am interested in developing and reasoning about safe algorithms, and I have been doing formal verification of concurrent objects with Iris framework on Coq proof assistant.
I have particular interest in verification under realistic and complex situations, e.g. weak memory models.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}

#### Publications

{% include publications.md author_id=person_id submitted=true %}
