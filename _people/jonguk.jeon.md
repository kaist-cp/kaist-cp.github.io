---
layout: people
background: /assets/images/kaist.jpg
title: Jonguk Jeon (전종욱)
excerpt: "Jonguk Jeon's website"
---

{%- assign person_id = "jonguk.jeon" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/jonguk.jeon.jpg" alt="{{ person.name }}">

I am an undergraduate intern at the [Concurrency and Parallelism Laboratory](https://www.fearless.systems). I'm passionate about impacting the world with computer science. I love creative HOWs in the field of computer science. A notable example is [AWS Aurora DB](https://www.amazon.science/publications/amazon-aurora-design-considerations-for-high-throughput-cloud-native-relational-databases). I was fascinated by the software techniques used to ensure high availability, despite relying on fundamentally fallible hardware. 

My interest in concurrency and parallelism was sparked by witnessing its impressive capabilities, especially its potential to accelerate processes up to 20 times faster than some of the most popular open-source projects. I chose to delve deeper into concurrency as it forms the backbone of large-scale systems that have a significant impact. Additionally, I am interested in foundational concepts such as type theory and systems architecture, aiming for common and fundamental impact.

I've honed my skills by leading projects and developing robust, enterprise-level products (with 400,000 MAU) at startups. 

Currently, I am focusing on the implementation and application of [Behavior-Oriented Concurrency](https://dl.acm.org/doi/10.1145/3622852) using Rust.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}

#### Experiences

- Backend Developer, Healingpaper, October 2020 ~ August 2023
- Frontend Developer, Tanker, October 2019 ~ Octover 2020
