---
layout: page
title: Bongjun Jang (장봉준)
excerpt: "Bongjun Jang's website"
---

{%- assign person_id = "bonjune.jang" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl}}/assets/bonjune.jang.jpg" alt="{{ person.name }}">

I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr) and [Mathematical Science](https://mathsci.kaist.ac.kr)**.

I am interested in Functional Programing and Computer Systems, believing cool languages can change the world: ([Rust](https://github.com/rust-lang/rust) and [F#](https://github.com/dotnet/fsharp))

Currently at KAIST GoN, Student Hacking Team.


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}