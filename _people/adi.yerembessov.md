---
layout: page
title: Adi Yerembessov
excerpt: "Adi Yerembessov's website"
---

{%- assign person_id = "adi.yerembessov" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl}}/assets/adi.yerembessov.jpg" alt="{{ person.name }}">
	
I am an **Undergraduate Student at [KAIST School of Computing](https://cs.kaist.ac.kr)**. The area of Computer Science that piqued my interest, during the years I've been studying at KAIST, is Computer Systems. For this reason, I was eager to join [Concurrency and Parallelism Laboratory](https://cp.kaist.ac.kr).

{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}

#### Experiences

- Teaching Assistant of Operating Systems and Lab course, KAIST, 2019 Spring Semester.


#### Awards and Honors

- Dean's List of the School of Computing, KAIST, 2018 Fall Semester.

