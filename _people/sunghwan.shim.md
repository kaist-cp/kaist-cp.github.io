---
layout: people
background: /assets/images/kaist.jpg
title: Sunghwan Shim (심성환)
excerpt: "Sunghwan Shim's website"
---

{%- assign person_id = "sunghwan.shim" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/sunghwan.shim.jpg" alt="{{ person.name }}">

I am a **Master Student at [Concurrency and Parallelism Laboratory]({{ site.url }})**. I am interested in developing concurrent design principles and building practical concurrent systems. Specifically, I am currently working on [AI serving systems]({{ site.baseurl }}{% link _projects/ai-system.md %}) and [Operating systems in Rust](https://github.com/kaist-cp/rv6) project.


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Experiences

- Backend developer, Team Dotout, March, 2017 - April, 2018

  (topic: live streaming service with enhanced user-streamer interaction)
