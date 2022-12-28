---
layout: people
background: /assets/images/kaist.jpg
title: Murad Bashirov
excerpt: "Murad Bashirov's website"
---

{%- assign person_id = "murad.bashirov" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/murad.bashirov.jpg" alt="{{ person.name }}">

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr)**.

I am interested in designing concurrent and parallel systems using **[Rust](https://rust-lang.org/)**.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}

#### Experiences

- Back-end engineer, Freelance, Weprosper Inc., September 2021 -- December 2021.

  (topic: Back-end development)


#### Awards and Honors

- Bronze medal, International distrubuted Physics Olympiad, Dec. 2021, Moscow, Russia.

- Bronze medal, European Physics Olympiad, Jun. 2021, Tailinn, Estonia.

- Silver medal, International Zhautikov Olympiad, Jan. 2021, Almaty, Khazakhstan.
