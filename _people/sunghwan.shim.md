---
layout: page
title: Sunghwan Shim (심성환)
excerpt: "Sunghwan Shim's website"
---

{%- assign person_id = "sunghwan.shim" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

I am a **Master Student at [Concurrency and Parallelism Laboratory]({{ site.url }})**. I am interested in verifying concurrent and parallel systems.


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Experiences

- Backend developer, Team Dotout, March, 2017 - April, 2018

  (topic: live streaming service with enhanced user-streamer interaction)
