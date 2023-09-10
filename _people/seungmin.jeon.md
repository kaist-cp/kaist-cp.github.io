---
layout: people
background: /assets/images/kaist.jpg
title: Seungmin Jeon (전승민)
excerpt: "Seungmin Jeon's website"
---

{%- assign person_id = "seungmin.jeon" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/seungmin.jeon.jpg" alt="{{ person.name }}">

I am a **Master Student at KAIST [School of Computing](https://cs.kaist.ac.kr)** at [Concurrency and Parallelism Laboratory](https://cp.kaist.ac.kr). 

My research focuses on enhancing the computing ecosystem for cutting-edge hardware, such as quantum computers and persistent memory.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}

#### Publications

{% include publications.md author_id=person_id submitted=true %}

- <span style="font-size: 110%; font-weight: bold;">Pre-processing Method for Bird Sound Classifier.</span>
  <br />
  Jaemin Kang, **Seungmin Jeon**, Hyungshin Kim.
  <br />
  Proceedings of 2020 IEMEK Symposium on Embedded Technology, July, 2020, pp. 40-41. (written in Korean)

- <span style="font-size: 110%; font-weight: bold;">A Malware Variants Detection Method Based on Malicious API Call Sequence.</span>
  <br />
  **Seungmin Jeon**, Woojin Joe, Hyongshik Kim.
  <br />
  Proceedings of Korea Software Congress 2019, December, 2019, pp. 1630-1632 (written in Korean)

#### Experiences

- Research intern, Mobile Distributed Computing Lab (Chungnam National University), September, 2020 - December, 2020

  (topic : behavioral control algorithm for autonomous robots)

- Research intern, Embedded System Lab (Chungnam National University), March, 2020 - June, 2020.

  (topic : sound-based bird classification)

- Development intern, Satrec Initiative, December, 2019 - February, 2020.

  (topic : various tool development)

- Research intern, System Architecture and Security Lab (Chungnam National University), June, 2019 - December, 2019

  (topic : identification of malicious code variants)
