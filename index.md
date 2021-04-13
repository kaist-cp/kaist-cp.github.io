---
layout: page
feature_text: |
  <h2 style="color: white;">Concurrency and Parallelism Laboratory</h2>
  <h4 style="color: white;">@ KAIST School of Computing</h4>
feature_image: "/assets/kaist.jpg"
excerpt: "Where theory meets practice"
---

{% capture pi_url %}{% include person_link.md person_id="jeehoon.kang" %}{% endcapture %}
{% assign pi_url = pi_url | strip %}

Welcome to Concurrency and Parallelism Laboratory at [KAIST](https://www.kaist.ac.kr) [School of
Computing](https://cs.kaist.ac.kr). **We are actively recruiting motivated students of all levels
interested in designing and verifying concurrent and parallel systems.** If you're interested,
please **read [an instruction]({{ site.baseurl }}/helpdesk/#advice-for-potential-lab-members) and
contact Jeehoon NOW.**

In the era of big data, artificial intelligence, and internet of things, humankind requires more and
more computing resources, but they are becoming more and more scarce due to the slowing of Dennard
scaling and Moore's law. The only way to meet the demand is to massively parallelize computing
resources to mitigate the damages of the slowing. So **we aim to design, implement, and verify such
massively parallel systems**, from microarchitectures to programming languages to algorithms,
thereby greatly improving the performance and significantly reducing power consumption over
conventional systems.

Our general strategy in attacking this goal is (1) to **holistically understand** the entire
computer systems; (2) to **develop abstraction layers** that realize the intrinsic parallelism of
the workloads while providing easy programming environment at the same time; and (3) to **formally
verify** such abstraction layers so that the users can use the them safely and fearlessly. See the
[Research](#research) page for more details.



<!-- ## News -->

<!-- <div id="news" style="width: 50%; height:auto;"> -->
<!--     <a class="twitter-timeline" href="https://twitter.com/kaist_cp?ref_src=twsrc%5Etfw">Tweets by kaist_cp</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>  -->
<!-- </div> -->



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

- {{ person.name }}
  [:house:]({{ person_url }})
  [:e-mail:](mailto:{{ mail_id }}@kaist.ac.kr)
  [:octocat:](https://github.com/{{ person.github }})
  ({{ person.title }})

{% endif %}
{% endfor %}

<!-- TODO: alumni? -->


## Research
<div id="research"></div>

We are designing concurrent and parallel systems that greatly improve performance and significantly
reduce power consumption, thereby serving as the basis for the upcoming era of massive data
processing. Our general strategy in attacking this goal is (1) to **holistically understand**
computer systems from microarchitectures to programming languages algorithms, and (2) to **develop
abstraction layers** that realize the intrinsic parallelism of the workloads while providing easy
programming environment at the same time. Specifically, we are working on the following projects:

- **Designing concurrent and parallel systems**: It is difficult to develop efficient and yet safe
  concurrent software/hardware, because efficient systems should allow concurrent accesses from
  multiple threads/components that complicate the reasoning of safety. We are developing **design
  patterns** for coordinating concurrent accesses, and using the design patterns, building practical
  concurrent systems. To this end, we are using
  [Crossbeam](https://github.com/crossbeam-rs/crossbeam) (a [Rust](https://www.rust-lang.org)
  concurrency library) and [RISC-V](https://riscv.org/) (an open-source ISA) as the
  testbed. Specifically, we are working on the following projects:

  + [AI hardware accelerators and their compilers]({{ site.baseurl }}{% link _projects/ai-accelerator.md %}) (with [FuriosaAI](https://www.furiosa.ai/))
  + Clean-slate operating systems for Android VMs (with Google)
  + Parallel networking systems
  + [Concurrent garbage collector]({{ site.baseurl }}{% link _projects/gc.md %})
  + Transactional systems based on [persistent memory]({{ site.baseurl }}{% link _projects/pmem.md %})

  <br />

- **Verifying concurrent and parallel systems**: It is difficult to ensure the safety of concurrent
  software/hardware by testing because they exhibit so many behaviors due to inherent nondeterminism
  arising from scheduling, optimization, or other factors. To address this problem, we are going to
  design verification techniques for proving the correctness of concurrent systems and verify
  real-world systems---such as operating systems, database systems, or cache coherence protocols,
  thereby answering the following research question: is verification more cost-effective than
  testing for concurrent systems?  Specifically, we are working on the following projects:

  + Modular verification theory for concurrency
  + Verification theory for persistent memory (with ETRI)
  + Garbage collector verification (with NRF)
  + Concurrent compiler verification (with NRF)



## Publications
<div id="publications"></div>

{% include publications.md %}
<!-- See the [publications]({{ site.baseurl }}{% link publications.md %}) page. -->



## Lectures
<div id="lectures"></div>

- [CS420: Compiler Design (2020 Spring)](https://github.com/kaist-cp/cs420)
- [CS492: Design and Analysis of Concurrent Programs (2020 Fall, 2019 Fall)](https://github.com/kaist-cp/cs492-concur)
- [CS500: Design and Analysis of Algorithm (2019 Spring)](https://github.com/kaist-cp/cs500-2019s)



## Contact
<div id="contact"></div>

- GitHub: [kaist-cp](https://github.com/kaist-cp)

- Rm. 4433 (Jeehoon) and Rm. 4441 (students), Bldg. E3-1

  School of Computing, KAIST

  291 Daehak-ro, Yuseong-gu

  Daejeon 34141, Korea

- +82-42-350-3578 (Jeehoon)
- +82-42-350-7878 (Students)
