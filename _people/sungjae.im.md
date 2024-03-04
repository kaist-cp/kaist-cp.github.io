---
layout: people
background: /assets/images/kaist.jpg
title: Sungjae Im (임성재)
---

{%- assign person_id = "sungjae.im" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/sungjae.im.jpg" alt="{{ person.name }}">

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr)**.

{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Awards and Honors

- Champion, ACM International Collegiate Programming Contest (ICPC) Regional Contest---Seoul, 2023.

- 2nd place, ACM International Collegiate Programming Contest (ICPC) Regional Contest---Seoul, 2021.

- Silver Medal, International Olympiad in Informatics (IOI), 2020.

