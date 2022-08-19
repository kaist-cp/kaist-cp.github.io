---
layout: people
background: /assets/images/kaist.jpg
title: Doehyun Baek (백도현)
excerpt: "Doehyun Baek's website"
---

{%- assign person_id = "doehyun.baek" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/doehyun.baek.jpg" alt="{{ person.name }}">

I am a student who wishes to pursue research on hardware-software codesign and systems programming in rust.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}