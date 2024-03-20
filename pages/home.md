---
layout: home
title: KAIST Concurrency and Parallelism
description: We design and verify innovative concurrent and parallel systems.
background: /assets/images/kaist.jpg
permalink: /
---

{% capture pi_url %}{% include person_link.md person_id="jeehoon.kang" %}{% endcapture %}
{% assign pi_url = pi_url | strip %}

{: .alert .alert-info}
**We are currently seeking enthusiastic students at all academic levels who are interested in designing and verifying concurrent and parallel systems.**
If this interests you, please **review these [instructions]({{ site.baseurl }}/join) and contact [Jeehoon]({{ site.baseurl }}/jeehoon.kang) as soon as possible.**


## Projects
<div id="projects"></div>

**In the era of big data, artificial intelligence, and the Internet of Things**, the demand for computing resources is rapidly increasing.
However, these resources are becoming scarce due to the slowing of Dennard scaling and Moore's law.
The most viable solution to address this shortage is to massively parallelize computing resources, helping to offset the impact of this slowdown. 

**Our objective is to design, implement, and verify such massively parallel systems**.
These systems range from microarchitectures to programming languages and algorithms, aiming to significantly enhance performance and reduce power consumption compared to conventional systems.

Our approach to achieving this goal involves three main strategies:
(1) **gaining a holistic understanding** of the entire computer systems;
(2) **designing abstraction layers** that harness the intrinsic parallelism of workloads while simultaneously offering an easy programming environment; and
(3) **formally verifying** these abstraction layers to ensure their safe and confident use by users.

Specifically, our focus is on the *design* and *verification* of concurrent and parallel systems:

- **Designing concurrent and parallel systems**: Developing efficient yet safe concurrent software and hardware is challenging. Efficient systems must support concurrent accesses by multiple threads or components, which complicates safety considerations. 
  
  **Therefore, we are developing design principles** for managing concurrent accesses and creating practical concurrent systems based on these principles. Our current projects include:

  + [AI serving systems]({{ site.baseurl }}{% link _projects/ai-system.md %}), optimized for NPUs in partnership with [FuriosaAI](https://www.furiosa.ai/)
  + [Operating systems in Rust](https://github.com/kaist-cp/rv6), designed for safety
  + [Persistent memory library]({{ site.baseurl }}{% link _projects/pmem.md %}), based on robust design principles
  + [Concurrent garbage collector]({{ site.baseurl }}{% link _projects/gc.md %}), focused on high throughput and low latency
  + [FPGA high-performance networking systems]({{ site.baseurl }}{% link _projects/fpga.md %}), emphasizing ease of programming

- **Verifying concurrent and parallel systems**: Ensuring the safety of concurrent software and hardware through testing alone is challenging due to the inherent non-determinism from scheduling, optimization, and other factors. 
  
  **Thus, we are developing verification techniques** to prove the correctness of concurrent systems and verify real-world systems like operating systems, database systems, or cache coherence protocols. This helps us explore whether verification is more cost-effective than testing for concurrent systems. Our verification projects include:

  + Persistent memory library
  + Strong specifications for concurrent data structures
  + Strong specifications for concurrent garbage collectors
  + Compilers for concurrent programs


### Publications
<div id="publications"></div>

{% include publications.md website=true %}


## People
<div id="people"></div>

<div class="container text-left">
<div class="row g-3">

{% for person in site.data.people %}
{% if person.status == "present" %}

{% assign person_id = person.id %}
{% capture person_url %}{% include person_url.md person_id=person_id %}{% endcapture %}

{% if person.kaist_id %}
{% assign mail_id = person.kaist_id %}
{% else %}
{% assign mail_id = person.id %}
{% endif %}

  <div class="col-5 col-md-2">
    {% if person.image %}
    <img style="width: 100%; " src="{{ person.image | relative_url }}" />
    {% else %}
    <img style="width: 100%; " src="{{ '/assets/images/question-mark.png' | relative_url }}" />
    {% endif %}
  </div>
  <div class="col-7 col-md-4 h5" id="{{ person.id }}">
    {{ person.name }}
    {% if person.role %}
    <br />
    <small class="text-muted">{{ person.role }}</small>
    {% endif %}
    {% include person_ext_links.md person_id=person.id %}
    <!-- {{ person.description | markdownify }} -->
  </div>

{% endif %}
{% endfor %}

</div>
</div>

<br />

### Alumni

<div class="container text-left">
<div class="row g-3">

{% for person in site.data.people %}
{% if person.status == "alumni" %}

{% assign person_id = person.id %}
{% capture person_url %}{% include person_url.md person_id=person_id %}{% endcapture %}

{% if person.kaist_id %}
{% assign mail_id = person.kaist_id %}
{% else %}
{% assign mail_id = person.id %}
{% endif %}

  <div class="col-md-6 h5" id="{{ person.id }}">
    {{ person.name }}, <small class="text-muted">{{ person.role }}</small>
    {% if person.job %}
    <br />
    <small class="text-muted h6"> (first occupation: {{ person.job }})</small>
    {% endif %}
    {% include person_ext_links.md person_id=person.id %}
    <!-- {{ person.description | markdownify }} -->
  </div>

{% endif %}
{% endfor %}

</div>
</div>

<br />




## Lectures
<div id="lectures"></div>

- [CS220: Programming Principles (2023-2021 Fall)](https://cp-git.kaist.ac.kr/cs220/cs220)
- [CS230: System Programming (2021 Spring)](https://cp-git.kaist.ac.kr/cs230/cs230)
- [CS420: Compiler Design (2023, 2022, 2020 Spring)](https://github.com/kaist-cp/cs420)
- [CS431: Concurrent Programming (2023-2019 Fall)](https://github.com/kaist-cp/cs431)
- [CS500: Design and Analysis of Algorithm (2019 Spring)](https://cp-git.kaist.ac.kr/jeehoon.kang/cs500)


## Contact
<div id="contact"></div>

- :office: **Place**:
  <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Rm. 4433 (Jeehoon) and Rm. 4441 (students), Bldg. E3-1
  <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;School of Computing, KAIST
  <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;291 Daehak-ro, Yuseong-gu
  <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Daejeon 34141, Korea
- :phone: **Phone**:
  <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+82-42-350-3578 (Jeehoon)
  <br />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;+82-42-350-7878 (Students)
- :speaking_head: **Comments**:
  <script src="https://utteranc.es/client.js"
    repo="kaist-cp/kaist-cp.github.io.comments"
    issue-term="pathname"
    theme="github-light"
        crossorigin="anonymous"
    async>
  </script>
