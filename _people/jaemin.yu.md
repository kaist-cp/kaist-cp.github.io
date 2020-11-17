---
layout: page
title: Jaemin Yu (유재민)
excerpt: "Jaemin Yu's website"
---

{%- assign person_id = "jaemin.yu" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr/)**.
I'm studying **[Rust](rust-lang.org)** and **[Coq](https://coq.inria.fr/)** to do a formal verification of the concurrent system.

{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}

#### Awards and Honors

- 8th place, International Collegiate Programming Contest (ICPC) Seoul Regional, 2018.
