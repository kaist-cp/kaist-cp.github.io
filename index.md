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
Computing](https://cs.kaist.ac.kr). We are designing and verifying concurrent and parallel systems,
from microarchitectures to programming languages to algorithms, that greatly improve performance and
significantly reduce power consumption, thereby serving as the basis for the upcoming era of massive
data processing.

**We are actively recruiting motivated students of all levels interested in designing and verifying
concurrent and parallel systems.** If interested, please send an email to {{ pi_url }}.



## News

#### 2019

- June, 2019: {%- include person_link.md person_id="kyeongmin.cho" %} joined as a master student,
  and {%- include person_link.md person_id="jaehwang.jung" %}, {%- include person_link.md
  person_id="jiseung.hong" %}, {%- include person_link.md
  person_id="adi.yerembessov" %} joined as undergraduate students. Welcome!
- February, 2019: Concurrency and Parallelism Laboratory was born.



## People

{% for person in site.data.people %}
{% if person.status == "present" %}

{% assign person_id = person.id %}
{% capture person_url %}{% include person_url.md person_id=person_id %}{% endcapture %}

- {{ person.name }}
  [:house:]({{ person_url }})
  [:e-mail:](mailto:{{ person.id }}@kaist.ac.kr)
  [:octocat:](https://github.com/{{ person.github }})
  ({{ person.title }})

{% endif %}
{% endfor %}



## Research

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

  + Parallel networking systems
  + Garbage collector
  + Programming environment for persistent memory

  <br />

- **Verifying concurrent and parallel systems**: It is difficult to ensure the safety of concurrent
  software/hardware by testing because they exhibit so many behaviors due to inherent nondeterminism
  arising from scheduling, optimization, or other factors. To address this problem, we are going to
  design verification techniques for proving the correctness of concurrent systems and verify
  real-world systems---such as operating systems, database systems, or cache coherence protocols,
  thereby answering the following research question: is verification more cost-effective than
  testing for concurrent systems?  Specifically, we are working on the following projects:

  + Modular verification theory for concurrent programs/compilers
  + Formal verfication of a hypervisor

  <br />

- **Designing compilers for deep learning hardware accelerator**: Deep learning accelerators like
  [Google TPU](https://cloud.google.com/tpu/) are specialized hardware purpose-built to achieve high
  performance by exploiting the intrinsic parallelism of the workloads. To better serve the target
  workloads, accelerators break the common abstraction layers established for general-purpose
  hardware like CPU. So it is difficult to design compilers for those accelerators that achieve
  programmability and efficiency at the same time. We are developing such a compiler in close
  collaboration with Furiosa AI.


## Publications

See the [publications]({{ site.baseurl }}{% link publications.md %}) page.


## Lectures

- [CS500: Design and Analysis of Algorithm (2019 Spring)](https://github.com/kaist-cp/cs500-2019s)
- [CS492: Design and Analysis of Concurrent Programs (2019 Fall)](https://github.com/kaist-cp/cs492-concur)


## Contact

- GitHub: [kaist-cp](https://github.com/kaist-cp)

- Rm. 4433 (Jeehoon) and Rm. 4441 (students), Bldg. E3-1

  School of Computing, KAIST

  291 Daehak-ro, Yuseong-gu

  Daejeon 34141, Korea

- +82-42-350-3578 (Jeehoon)
- +82-42-350-7878 (Students)
