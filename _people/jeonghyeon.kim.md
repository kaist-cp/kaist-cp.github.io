---
layout: people
background: /assets/images/kaist.jpg
title: Jeonghyeon Kim (김정현)
excerpt: "Jeonghyeon Kim's website"
---

{%- assign person_id = "jeonghyeon.kim" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/jeonghyeon.kim.jpg" alt="{{ person.name }}">

I am an **Undergraduate Intern at [Concurrency and Parallelism Laboratory]({{ site.url }}), [KAIST School of Computing](https://cs.kaist.ac.kr)**. After I received my bachelor's degree in [Computer Science from the University of Seoul](https://cs.uos.ac.kr), I joined Concurrency and Parallelism Laboratory to find a better way to reason concurrent and parallel systems.

Currently, I am interested in designing and verifying concurrent systems such as safe memory reclamation techniques or file systems.


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Experiences

- Research Intern, Intelligent Robot Lab, University of Seoul, December 2020 - June 2021.
  - Topic: Speaker Verification with d-vector, x-vector and Prototypical Network
- Research Intern, Global Urban & Infrastructure Research Center, University of Seoul, September 2020 - November 2022.
  - Topic: Development of Real-Time Analysis and Monitoring Technology for Traffic Safety Big Data (with Korea Expressway
Corporation)


#### Awards and Honors

- Academic Excellence Award (Top Student in Spring 2020), University of Seoul, 2020.
- 14th place (by ICPC rules), International Collegiate Programming Contest (ICPC) Seoul Regional, 2020.
- The Special Award in Auto-driving Car, The World Embedded Software Contest 2020, Hyundai & Ministry of Trade, Industry and Energy, 2021.
- The Encouragement Award, ‘22 Hyundai Mobis Algorithm Competition, Hyundai Mobis, 2022.