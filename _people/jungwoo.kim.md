---
layout: people
background: /assets/images/kaist.jpg
title: Jungwoo Kim (김정우)
excerpt: "Jungwoo Kim's website"
---

{%- assign person_id = "jungwoo.kim" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/jungwoo.kim.jpg" alt="{{ person.name }}">

I am a **research scientist at [CASYS KAIST](https://casyslab.kaist.ac.kr/)** supervised by [Prof. Jaehyuk Huh](https://jaehyuk-huh.github.io/index.html).
I received an M.S. degree in 2023 and a B.S. degree in 2021, both from KAIST.
My primary research area includes accelerated systems for ML training and hardware-software co-design for ML applications.

During my undergraduate studies, I had the privilege of participating in the [rv6](https://github.com/kaist-cp/rv6) project and being supervised by [Prof. Jeehoon Kang](https://cp.kaist.ac.kr/jeehoon.kang/).

Please be aware that this page is no longer updated since August 2023. For the latest information about me, kindly visit [my personal webpage](https://sites.google.com/view/jungwookim).


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


<!--

#### Calendar

<div class="responsive-iframe-container big-container">
    <iframe src="https://calendar.google.com/calendar/embed?showTitle=0&amp;showPrint=0&amp;mode=WEEK&amp&amp;wkst=1&amp;bgcolor=%23FFFFFF&amp;src=jeehoon.kang%40cp.kaist.ac.kr&amp;color=%23125A12&amp;ctz=Asia%2FSeoul" style="border-width:0; margin-top:15pt;" frameborder="0" scrolling="no"></iframe>
</div>
<div class="responsive-iframe-container small-container" style="height: 1000;">
    <iframe src="https://calendar.google.com/calendar/embed?showTitle=0&amp;showPrint=0&amp;mode=AGENDA&amp&amp;wkst=1&amp;bgcolor=%23FFFFFF&amp;src=jeehoon.kang%40cp.kaist.ac.kr&amp;color=%23125A12&amp;ctz=Asia%2FSeoul" style="border-width:0" frameborder="0" scrolling="no"></iframe>
</div>

-->
