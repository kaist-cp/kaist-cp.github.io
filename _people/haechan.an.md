---
layout: people
background: /assets/images/kaist.jpg
title: Haechan An (안해찬)
excerpt: "Haechan An's website"
---

{%- assign person_id = "haechan.an" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/haechan.an.jpg" alt="{{ person.name }}">

I am **Master's student at [KAIST School of Computing](https://cs.kaist.ac.kr/)**.
The followings are my interests: **Programming language theories** including formal semantics, abstract interpretation, interactive theorem proving and concurrency; **Building complex systems** such as compilers in safe and usable languages like Rust; Additionally, applying **learning-based techniques** to the above area.

I've worked on building [AI serving systems](https://www.fearless.systems/ai-system) and AI-based automation of formal verification.
Now, I'm starting a project on deep learning compilers. 


Details of my experiences are at [my personal webpage](https://anhaechan.github.io/).


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}
