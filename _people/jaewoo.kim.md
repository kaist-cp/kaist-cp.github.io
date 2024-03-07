---
layout: people
background: /assets/images/kaist.jpg
title: Jaewoo Kim (김재우)
excerpt: "Jaewoo Kim's website"
---

{%- assign person_id = "jaewoo.kim" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/jaewoo.kim.jpg" alt="{{ person.name }}">

I am a **Master's Student at [KAIST School of Computing](https://cs.kaist.ac.kr/)**.
I am interested in formally defining and proving program behavior using logic.


{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}

#### Publications

{% include publications.md author_id=person_id submitted=true %}

#### Experiences

- Intern, Programming Systems Lab, Kaist, December 2021 ~ Feburary 2022 \
  (topic: Developing Infer-based static analyzer for checking type confusion bugs)

- Client developer, Shiftup Corp, July 2021 - August 2021.
