---
layout: people
background: /assets/images/kaist.jpg
title: Kyeongmin Cho (조경민)
excerpt: "Kyeongmin Cho's website"
---

{%- assign person_id = "kyeongmin.cho" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/kyeongmin.cho.jpg" alt="{{ person.name }}">

I am a **Ph.D. Student at [Concurrency and Parallelism Laboratory]({{ site.url }}), [KAIST School of Computing](https://cs.kaist.ac.kr)**. I
am very fortunate to be advised by [Prof. Jeehoon Kang]({{ site.baseurl }}{% include person_url.md person_id="jeehoon.kang" %}). Prior to KAIST, I received my B.S. in CSE and B.A. in Philosophy from Inha University.

My primary research interests lie in the area of concurrency, persistency and programming languages. In particular, I am interested in developing and verifying design patterns for coordinating concurrent accesses, and using the design patterns, building practical concurrent systems.


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Publications

{% include publications.md author_id=person_id submitted=true %}

#### Professional Activities

- [2022 POPL AEC](https://popl22.sigplan.org/committee/POPL-2022-artifact-evaluation-artifact-evaluation-comittee) member

#### Experiences

- Director, Marketit Inc., July, 2016 - August, 2017.

- Mentee, Software Maestro, June, 2015 – June, 2016.

#### Awards and Honors

- NAVER PhD Fellowship Award, NAVER Corp., 2021.

- Grand Prize, Capstone Project Competition, Dept. of Computer Science and Engineering, Inha University, 2018.

- 14th place, ACM International Collegiate Programming Contest (ICPC) Regional Contest---Daejeon, 2014.

- Kiwoom Securities Financial Scholarship, Kiwoom Securities Corp., 2014 - 2015.

#### Calendar

<div class="responsive-iframe-container big-container">
    <iframe src="https://calendar.google.com/calendar/embed?showTitle=0&amp;showPrint=0&amp;mode=WEEK&amp&amp;wkst=1&amp;bgcolor=%23FFFFFF&amp;src=kyeongmin.cho%40cp.kaist.ac.kr&amp;color=%23125A12&amp;ctz=Asia%2FSeoul" style="border-width:0; margin-top:15pt;" frameborder="0" scrolling="no"></iframe>
</div>
<div class="responsive-iframe-container small-container" style="height: 1000;">
    <iframe src="https://calendar.google.com/calendar/embed?showTitle=0&amp;showPrint=0&amp;mode=AGENDA&amp&amp;wkst=1&amp;bgcolor=%23FFFFFF&amp;src=kyeongmin.cho%40cp.kaist.ac.kr&amp;color=%23125A12&amp;ctz=Asia%2FSeoul" style="border-width:0" frameborder="0" scrolling="no"></iframe>
</div>
