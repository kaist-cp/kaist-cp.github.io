---
layout: people
background: /assets/images/kaist.jpg
title: Seungmin Jeon (전승민)
excerpt: "Seungmin Jeon's website"
---

{%- assign person_id = "seungmin.jeon" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/seungmin.jeon.jpg" alt="{{ person.name }}">

I am an **Undergraduate Student at [Chungnam National University, Department of Computer Science and Engineering](http://cse.cnu.ac.kr/)**. I joined [Concurrency and Parallelism Laboratory](https://cp.kaist.ac.kr) because I'm interested in designing concurrent and parallel systems and studying how to research these topics.

Thankfully, I am working on designing a practical [persistent memory library](https://cp.kaist.ac.kr/pmem), one of my interesting topics.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}

#### Experiences

- Research intern, Mobile Distributed Computing Lab (Chungnam National University), September, 2020 - December, 2020

  (topic : behavioral control algorithm for autonomous robots)

- Research intern, Embedded System Lab (Chungnam National University), March, 2020 - June, 2020.

  (topic : sound-based bird classification)

- Development intern, Satrec Initiative, December, 2019 - February, 2020.

  (topic : various tool development)

- Research intern, System Architecture and Security Lab (Chungnam National University), June, 2019 - December, 2019

  (topic : identification of malicious code variants)


#### Publications

{% include publications.md author_id=person_id submitted=true %}

* Jaemin Kang, **Seungmin Jeon**, Hyungshin Kim. Pre-processing Method for Bird Sound Classifier. Proceedings of 2020 IEMEK Symposium on Embedded Technology, July, 2020, pp. 40-41. (written in Korean)

* **Seungmin Jeon**, Woojin Joe, Hyongshik Kim. A Malware Variants Detection Method Based on Malicious API Call Sequence, Proceedings of Korea Software Congress 2019, December, 2019 , pp. 1630-1632 (written in Korean)
