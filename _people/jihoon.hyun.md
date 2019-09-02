---
layout: page
title: Jihoon Hyun (현지훈)
excerpt: "Jihoon Hyun's website"
---

{%- assign person_id = "jihoon.hyun" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

I am an **undergraduate student at [KAIST School of Computing](https://cs.kaist.ac.kr)**.


#### Contact

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}

- Place : Rm. 4441, Bldg. E3-1, KAIST (+82-42-350-7878)

<!--
#### Calendar

<div class="responsive-iframe-container big-container">
    <iframe src="https://calendar.google.com/calendar/embed?showTitle=0&amp;showPrint=0&amp;mode=WEEK&amp&amp;wkst=1&amp;bgcolor=%23FFFFFF&amp;src=jiseung.hong%40cp.kaist.ac.kr&amp;color=%23125A12&amp;ctz=Asia%2FSeoul" style="border-width:0; margin-top:15pt;" frameborder="0" scrolling="no"></iframe>
</div>
<div class="responsive-iframe-container small-container" style="height: 1000;">
    <iframe src="https://calendar.google.com/calendar/embed?showTitle=0&amp;showPrint=0&amp;mode=AGENDA&amp&amp;wkst=1&amp;bgcolor=%23FFFFFF&amp;src=jiseung.hong%40cp.kaist.ac.kr&amp;color=%23125A12&amp;ctz=Asia%2FSeoul" style="border-width:0" frameborder="0" scrolling="no"></iframe>
</div>
-->