---
layout: people
background: /assets/images/kaist.jpg
title: Chunmyong Park (박천명)
excerpt: "Chunmyong Park's website"
---

{%- assign person_id = "chunmyong.park" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl }}/assets/images/people/chunmyong.park.jpeg" alt="{{ person.name }}">

I am a **Ph.D. Student at [Concurrency and Parallelism Laboratory]({{ site.url }}), [KAIST School of Computing](https://cs.kaist.ac.kr)**. I am delighted to be advised by [Prof. Jeehoon Kang]({{ site.baseurl }}{% include person_url.md person_id="jeehoon.kang" %}).

My research interests are in constructing the AI serving systems using heterogeneous processors such as CPU, GPU, NPU, etc. In particular, I am focused on designing resource managers and schedulers for the system to better serve real-world workloads. I am currently working with [FuriosaAI](https://www.furiosa.ai/) for this research. If you want to know more about this research topic, please refer to this [link](https://cp.kaist.ac.kr/ai-system).


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Publications

{% include publications.md author_id=person_id submitted=true %}


#### Experiences

- Intern, FuriosaAI, July, 2020 - August, 2020.

  - Designing next-generation AI serving system using NPU

- Intern, KakaoBrain, July, 2019 - August, 2019.

  - torchlars: A [LARS(Layer-wise Adaptive Rate Scaling)](https://arxiv.org/abs/1708.03888) implementation in PyTorch, [github](https://github.com/kakaobrain/torchlars), [blog post](https://www.kakaobrain.com/blog/113)

- Intern, DeepBio, January, 2018 - February, 2018.

  - [CAMELYON17](https://camelyon17.grand-challenge.org/) project: Designing the deep learning model for detection and classification of breast cancer metastases, [github](https://github.com/cmpark0126/CamelyonTask)

- Research Assistant, Deep Learning Lab (director: Prof. Injung Kim), Handong Global University, March, 2017 – June, 2019.

  - WICWIU: A deep learning library in C/C++, [github], [thesis]


#### Awards and Honors

- Best Paper Award, Korea Computer Congress (KCC), 2018.


#### Calendar

<div class="responsive-iframe-container big-container">
    <iframe src="<iframe src="https://calendar.google.com/calendar/embed?height=600&amp;wkst=1&amp;bgcolor=%23ffffff&amp;ctz=Asia%2FSeoul&amp;src=Y2h1bm15b25nLnBhcmtAY3Aua2Fpc3QuYWMua3I&amp;src=a28uc291dGhfa29yZWEjaG9saWRheUBncm91cC52LmNhbGVuZGFyLmdvb2dsZS5jb20&amp;color=%239E69AF&amp;color=%230B8043&amp;showTz=1&amp;showCalendars=0&amp;showTabs=0&amp;mode=WEEK&amp;showDate=0&amp;showTitle=0&amp;showPrint=0" style="border-width:0; margin-top:15pt;" width="800" height="600" frameborder="0" scrolling="no"></iframe>
</div>
<div class="responsive-iframe-container small-container" style="height: 1000;">
    <iframe src="https://calendar.google.com/calendar/embed?height=600&amp;wkst=1&amp;bgcolor=%23ffffff&amp;ctz=Asia%2FSeoul&amp;src=Y2h1bm15b25nLnBhcmtAY3Aua2Fpc3QuYWMua3I&amp;src=a28uc291dGhfa29yZWEjaG9saWRheUBncm91cC52LmNhbGVuZGFyLmdvb2dsZS5jb20&amp;color=%239E69AF&amp;color=%230B8043&amp;showTz=1&amp;showCalendars=0&amp;showTabs=0&amp;mode=WEEK&amp;showDate=0&amp;showTitle=0&amp;showPrint=0" style="border-width:0; margin-top:15pt;" width="800" height="600" frameborder="0" scrolling="no"></iframe>
</div>
