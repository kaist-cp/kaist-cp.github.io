---
layout: home
title: Concurrency and Parallelism
description: We design and verify innovative concurrent and parallel systems.
background: /assets/images/kaist.jpg
permalink: /
---

{% capture pi_url %}{% include person_link.md person_id="jeehoon.kang" %}{% endcapture %}
{% assign pi_url = pi_url | strip %}

{: .alert .alert-info}
**We're actively recruiting motivated students of all levels
interested in designing and verifying concurrent and parallel systems.** If you're interested,
please **read this [instruction]({{ site.baseurl }}/join) and
contact Jeehoon ASAP.**


<!-- Welcome to Concurrency and Parallelism Laboratory at [KAIST](https://www.kaist.ac.kr) [School of Computing](https://cs.kaist.ac.kr)! -->

## Research
<div id="research"></div>

**In the era of big data, artificial intelligence, and internet of things**, humankind requires more and
more computing resources, but they are becoming more and more scarce due to the slowing of Dennard
scaling and Moore's law. The only way to meet the demand is to massively parallelize computing
resources to mitigate the damages of the slowing. 

**So we aim to design, implement, and verify such massively parallel systems**, from
microarchitectures to programming languages to algorithms, that greatly improves the performance and
significantly reduces power consumption over conventional systems.

Our general strategy in attacking this goal is (1) to **holistically understand** the entire
computer systems; (2) to **design abstraction layers** that realize the intrinsic parallelism of
the workloads while providing easy programming environment at the same time; and (3) to **formally
verify** such abstraction layers so that the users can use the them safely and fearlessly.


### Projects

Specifically, we are working on *design* and *verification* of concurrent and parallel systems:

- **Designing concurrent and parallel systems**: It is difficult to develop efficient and yet safe
  concurrent software and hardware, because efficient systems should allow concurrent accesses from
  multiple threads or components that complicate the reasoning of safety. 
  
  **So we are developing design principles** for coordinating concurrent accesses, and based on the
  design principles, building practical concurrent systems. Specifically, we are building:

  + [AI serving systems]({{ site.baseurl }}{% link _projects/ai-system.md %}), optimized for NPUs (with [FuriosaAI](https://www.furiosa.ai/))
  + [Operating systems in Rust](https://github.com/kaist-cp/rv6), safe by construction (with Google)
  + [Persistent memory library]({{ site.baseurl }}{% link _projects/pmem.md %}), with solid design principles (with ETRI)
  + [Concurrent garbage collector]({{ site.baseurl }}{% link _projects/gc.md %}), with high throughput and low latency
  + [FPGA high-performance networking systems]({{ site.baseurl }}{% link _projects/fpga.md %}), easily programmable

    <!-- To this end, we are using [Crossbeam](https://github.com/crossbeam-rs/crossbeam) (a -->
    <!-- [Rust](https://www.rust-lang.org) concurrency library) and [RISC-V](https://riscv.org/) (an -->
    <!-- open-source ISA) as the testbed. -->

- **Verifying concurrent and parallel systems**: It is difficult to ensure the safety of concurrent
  software and hardware by testing because they exhibit so many behaviors due to inherent
  nondeterminism arising from scheduling, optimization, or other factors. 
  
  **So we are designing verification techniques** for proving the correctness of concurrent systems
  and verify real-world systems---such as operating systems, database systems, or cache coherence
  protocols, thereby answering the following research question: is verification more cost-effective
  than testing for concurrent systems? Specifically, we are verifying:

  + Persistent memory library (with ETRI)
  + Strong specification of concurrent data structures (with MPI-SWS)
  + Strong specification of concurrent garbage collectors
  + Compilers for concurrent programs


### Publications
<div id="publications"></div>

{% include publications.md website=true %}


## People
<div id="people"></div>

{% for person in site.data.people %}
{% if person.status == "present" %}

{% assign person_id = person.id %}
{% capture person_url %}{% include person_url.md person_id=person_id %}{% endcapture %}

{% if person.kaist_id %}
{% assign mail_id = person.kaist_id %}
{% else %}
{% assign mail_id = person.id %}
{% endif %}

  <div class="media team-person">
    {% if person.image %}
    <img class="mr-3" style="width: 15%;" src="{{ person.image | relative_url }}">
    {% else %}
    <img class="mr-3" style="width: 15%;" src="{{ site.baseurl }}assets/images/question-mark.png">
    {% endif %}
    <div class="media-body">
      <h5 id="{{ person.id }}">
        {{ person.name }}
        {% if person.role %}
        <small class="text-muted">| {{ person.role }}</small>
        {% endif %}
      </h5>

      <ul class="list-inline">
        <li class="list-inline-item">
          <a href="{{ person_url }}"><i class="fa fa-home"></i></a>
        </li>

        {% if person.orcid %}
        <li class="list-inline-item">
          <a href="https://orcid.org/{{ person.orcid }}"><img class="orcid" src="{{ '/assets/theme/img/orcid.png' | relative_url }}"></a>
        </li>
        {% endif %}

        <li class="list-inline-item">
          <a href="mailto:{{ mail_id }}@kaist.ac.kr"><i class="fa fa-envelope"></i></a>
        </li>

        {% if person.twitter %}
        <li class="list-inline-item">
          <a href="https://twitter.com/{{ person.twitter }}"><i class="fa fa-twitter"></i></a>
        </li>
        {% endif %}

        {% if person.github %}
        <li class="list-inline-item">
          <a href="https://github.com/{{ person.github }}"><i class="fa fa-github"></i></a>
        </li>
        {% endif %}
      </ul>

      {{ person.description | markdownify }}
    </div>
  </div>

{% endif %}
{% endfor %}

<br />

### Alumni

{% for person in site.data.people %}
{% if person.status == "alumni" %}

{% assign person_id = person.id %}
{% capture person_url %}{% include person_url.md person_id=person_id %}{% endcapture %}

{% if person.kaist_id %}
{% assign mail_id = person.kaist_id %}
{% else %}
{% assign mail_id = person.id %}
{% endif %}

  <div class="media team-person">
    <div class="media-body">
      <h5 id="{{ person.id }}">
        {{ person.name }}
        {% if person.role %}
        <small class="text-muted">| {{ person.role }}</small>
        {% endif %}
        {% if person.job %}
        <small class="text-muted">| first occupation: {{ person.job }}</small>
        {% endif %}
      </h5>

      <ul class="list-inline">
        <li class="list-inline-item">
          <a href="{{ person_url }}"><i class="fa fa-home"></i></a>
        </li>

        {% if person.orcid %}
        <li class="list-inline-item">
          <a href="https://orcid.org/{{ person.orcid }}"><img class="orcid" src="{{ '/assets/theme/img/orcid.png' | relative_url }}"></a>
        </li>
        {% endif %}

        <li class="list-inline-item">
          <a href="mailto:{{ mail_id }}@kaist.ac.kr"><i class="fa fa-envelope"></i></a>
        </li>

        {% if person.twitter %}
        <li class="list-inline-item">
          <a href="https://twitter.com/{{ person.twitter }}"><i class="fa fa-twitter"></i></a>
        </li>
        {% endif %}

        {% if person.github %}
        <li class="list-inline-item">
          <a href="https://github.com/{{ person.github }}"><i class="fa fa-github"></i></a>
        </li>
        {% endif %}
      </ul>

      {{ person.description | markdownify }}
    </div>
  </div>

{% endif %}
{% endfor %}

<br />


<!-- TODO: alumni? -->


## Lectures
<div id="lectures"></div>

- [CS220: Programming Principles (2022, 2021 Fall)](https://cp-git.kaist.ac.kr/cs220/cs220)
- [CS230: System Programming (2021 Spring)](https://cp-git.kaist.ac.kr/cs230/cs230)
- [CS420: Compiler Design (2023, 2022, 2020 Spring)](https://github.com/kaist-cp/cs420)
- [CS431: Concurrent Programming (2022-2019 Fall)](https://github.com/kaist-cp/cs431)
- [CS500: Design and Analysis of Algorithm (2019 Spring)](https://cp-git.kaist.ac.kr/jeehoon.kang/cs500)


## Contact
<div id="contact"></div>

- **Address**: Rm. 4433 (Jeehoon) and Rm. 4441 (students), Bldg. E3-1
  <br />
  School of Computing, KAIST
  <br />
  291 Daehak-ro, Yuseong-gu
  <br />
  Daejeon 34141, Korea
- **Phone**: +82-42-350-3578 (Jeehoon), +82-42-350-7878 (Students)
- [**Helpdesk**]({{ site.baseurl }}{% link pages/helpdesk.md %})
- **Comments**: Do you want to talk to us here? Feel free to leave a comment!
  <script src="https://utteranc.es/client.js"
    repo="kaist-cp/kaist-cp.github.io.comments"
    issue-term="pathname"
    theme="preferred-color-scheme"
    crossorigin="anonymous"
    async>
  </script>
