---
layout: page
title: Hyunsu Kim (김현수)
excerpt: "Hyunsu Kim's website"
---

{%- assign person_id = "hyunsu.kim" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl}}/assets/hyunsu.kim.jpeg" alt="{{ person.name }}">

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr)**.
I once used to be interested in machine learning and data mining algorithms.
Now, I'm getting attracted to concurrent programming that really drives the scalable system and applications.
Trying to become **[Rust](rust-lang.org)** enthusiast:fire:


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Experiences

- Front-end web developer, [Classum](https://classum.com), February, 2019 - December, 2019.


#### Publications

- Data Cleaning for Accurate, Fair, and Robust Models: A Big Data - AI Integration Approach [Short Paper]
Kihyun Tae; Yuji Roh; Young Hun Oh; *Hyunsu Kim*; Steven Whang (KAIST)

#### Awards and Honors

- Software Development Awards, Qualcomm-KAIST Innovation Awards Committee, 2018.