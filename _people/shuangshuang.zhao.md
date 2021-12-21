---
layout: people
background: /assets/images/kaist.jpg
title: Shuangshuang Zhao
excerpt: "Shuangshuang Zhao's website"
---

{%- assign person_id = "shuangshuang.zhao" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/shuangshuang.zhao.jpg" alt="{{ person.name }}">

I am a **PhD student at [Concurrency and Parallelism Laboratory]({{ site.url }}), [KAIST School of Computing](https://cs.kaist.ac.kr)**. I am really grateful to be adviced by [Prof. Jeehoon Kang]({{ site.baseurl }}{% include person_url.md person_id="jeehoon.kang" %}). Prior to KAIST, I received my M.S from Concordia University (Montreal, Canada). I am interested in understanding how different systems work thoroughly, and then make them secure and fast.


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Experiences

- R&D Engineer, Immux, June, 2018 - May, 2021.
  - Build an immutable storage engine from scratch. 

- Agile Software Engineer, Tribalscale, Apr, 2016 - Oct, 2017.
  - I build all different kinds of applications (mobile apps, full stack, voice platform).


#### Publications

{% include publications.md author_id=person_id submitted=true %}

#### Open Source Contributions

- [Immux](https://github.com/immux/immux): An immutable storage engine written in [Rust](https://www.rust-lang.org)

- [Sled](https://github.com/spacejam/sled/pull/1190): A lock free embedded database.

#### Awards and Honors

- Distinguished Graduate Student, Department of Computer Science and Software Engineering, Concordia University, 2015.

- Winner of Hack Western II Hackathon out of 200 teams, [Major League Hack](https://en.wikipedia.org/wiki/Major_League_Hacking), 2015.

#### Calendar

<div class="responsive-iframe-container big-container">
    <iframe src="https://calendar.google.com/calendar/embed?wkst=1&bgcolor=%23ffffff&ctz=America%2FVancouver&showTitle=0&showNav=1&showPrint=0&mode=WEEK&showTabs=1&src=c2h1YW5nc2h1YW5nLnpoYW9AY3Aua2Fpc3QuYWMua3I&color=%23039BE5" style="border-width: 0, margin-top:15pt;" frameborder="0" scrolling="no"></iframe>
</div>
<div class="responsive-iframe-container small-container" style="height: 1000;">
    <iframe src="https://calendar.google.com/calendar/embed?wkst=1&bgcolor=%23ffffff&ctz=America%2FVancouver&showTitle=0&showNav=1&showPrint=0&mode=WEEK&showTabs=1&src=c2h1YW5nc2h1YW5nLnpoYW9AY3Aua2Fpc3QuYWMua3I&color=%23039BE5" style="border-width: 0, margin-top:15pt;" frameborder="0" scrolling="no"></iframe>
</div>
