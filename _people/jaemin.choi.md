---
layout: people
background: /assets/images/kaist.jpg
title: Jaemin Choi (최재민)
excerpt: "Jaemin Choi's website"
---

{%- assign person_id = "jaemin.choi" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/jaemin.choi.jpg" alt="{{ person.name }}">

I am a **Master Student at [KAIST School of Computing](https://cs.kaist.ac.kr/)**. I am studying formal verification of concurrent systems - in particular, I'm working on formal verification of concurrent real-world programs

{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Publications

{% include publications.md author_id=person_id submitted=true %}

#### Awards and Honors

- 2nd place (by ICPC rules), International Collegiate Programming Contest (ICPC) Seoul Regional, 2020.

- 3rd place award, Samsung Collegiate Programming Cup (SCPC), 2020.
