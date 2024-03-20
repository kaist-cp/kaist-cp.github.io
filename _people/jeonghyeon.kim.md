---
layout: people
background: /assets/images/kaist.jpg
title: Jeonghyeon Kim (김정현)
excerpt: "Jeonghyeon Kim's website"
---

{%- assign person_id = "jeonghyeon.kim" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/jeonghyeon.kim.jpg" alt="{{ person.name }}">

I'm currently pursuing a **Master's degree at the [Graduate School of AI Semiconductor, KAIST](https://aisemi.kaist.ac.kr/)**. After earning my bachelor's degree in [Computer Science from the University of Seoul](https://cs.uos.ac.kr), I joined the Concurrency and Parallelism Laboratory to explore more effective methods for reasoning about concurrent and parallel systems.

I kicked off my research journey by contributing to [Jaehwang's HP++ project]({{ site.baseurl }}/gc), an extension of *Hazard pointers* designed for enhanced applicability. Building on that, my current focus revolves around devising an innovative approach to further enhance the hazard pointer scheme, aiming to achieve both improved performance and robustness.
<!-- TODO: Talk more about "a new way to improve hazard pointer" after finishing the work... -->

Additionally, I have a keen interest in verifying critical systems, particularly distributed systems and file systems. Presently, I am collaborating with [Northeastern University](https://www.northeastern.edu/) on developing a framework for verifying the safety and liveness of a distributed key-value store.


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Publications

{% include publications.md author_id=person_id submitted=true %}


#### Awards and Honors

- Academic Excellence Award (Top Student in Spring 2020), University of Seoul, 2020.

- 14th place (by ICPC rules), International Collegiate Programming Contest (ICPC) Seoul Regional, 2020.

- The Special Award in Auto-driving Car, The World Embedded Software Contest 2020, Hyundai & Ministry of Trade, Industry and Energy, 2021.

- The Encouragement Award, ‘22 Hyundai Mobis Algorithm Competition, Hyundai Mobis, 2022.

- 2nd place, Goorm Algorithm Monday Challenge, Goorm, 2022.
