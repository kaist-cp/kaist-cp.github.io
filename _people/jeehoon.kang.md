---
layout: page
title: Jeehoon Kang (강지훈)
excerpt: "Jeehoon Kang's website"
---

{%- assign person_id = "jeehoon.kang" %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<img align="right" style="width: 30%; padding-left: 3%;" src="{{ site.baseurl}}/assets/jeehoon.kang.jpg" alt="{{ person.name }}">

I am an **Assistant Professor at [KAIST School of Computing](https://cs.kaist.ac.kr)** and the
**Principal Investigator of [Concurrency and Parallelism Laboratory](https://cp.kaist.ac.kr)**. I
received my Ph.D. from Seoul National University under the supervision of [Prof. Chung-Kil
Hur](https://sf.snu.ac.kr/gil.hur). I am designing and verifying concurrent and parallel systems,
from microarchitectures to programming languages to algorithms, that greatly improve performance and
significantly reduce power consumption, thereby serving as the basis for the upcoming era of massive
data processing.

**I am recruiting motivated students of all levels interested in designing and verifying concurrent
and parallel systems.** See the [main page]({{ site.baseurl }}) and the [helpdesk](https://github.com/kaist-cp/helpdesk/#advice-for-potential-lab-members) for more details. Most crucially: **contact Jeehoon NOW**.


{% include person_contact.md person_id=person_id %}


{% include person_education.md person_id=person_id %}


#### Experiences

- Chief R&D Officer and Founder, Furiosa AI, September, 2017 - current.

  (topic: deep learning accelerator and its compiler)

- Intern, MPI-SWS, September, 2015 - December, 2015

  (topic: relaxed-memory concurrency, advisor: Dr. [Derek Dreyer](https://people.mpi-sws.org/~dreyer/))

- Software Engineer Intern, Google Korea, June, 2008 – August, 2008.

  (topic: machine translation)


#### Publications

See the [research]({{ site.baseurl }}{% link index.md %}#research) and [publications]({{ site.baseurl }}{%
link publications.md %}) pages.


#### Lectures

- [CS230: System Programming (2021 Spring)](https://github.com/kaist-cp/cs230)
- [CS420: Compiler Design (2020 Spring)](https://github.com/kaist-cp/cs420)
- [CS492: Design and Analysis of Concurrent Programs (2020 Fall, 2019 Fall)](https://github.com/kaist-cp/cs492-concur)
- [CS500: Design and Analysis of Algorithm (2019 Spring)](https://github.com/kaist-cp/cs500-2019s)


#### Professional Activities

- Program Committee Chairs: [2021 POPL AEC](https://popl21.sigplan.org/), [2020 POPL AEC](https://popl20.sigplan.org/)

- Program Committee Members: 2022 ESOP, [2021 HOPE](https://icfp21.sigplan.org/home/hope-2021), [2021 POPL](https://popl21.sigplan.org/), 2021 OOPSLA, [2020 ICSE NIER](https://conf.researchr.org/home/icse-2020), [2020 ICSE
  SEIP](https://conf.researchr.org/home/icse-2020), [2020 ASPLOS
  (ERC)](https://asplos-conference.org/), [2019 POPL AEC](https://popl19.sigplan.org/)
  
- Others: [2022 POPL](https://popl22.sigplan.org/series/POPL) Student Research Competition Co-Chair, 2022 CGO Proceedings Chair, [2021 CGO](https://conf.researchr.org/home/cgo-2021) Proceedings Chair, [2020 ICSE](https://conf.researchr.org/home/icse-2020) Virtualization Technology Chair


#### Open Source Contributions

- [Crossbeam](https://github.com/crossbeam-rs/crossbeam): a concurrency library in [Rust](https://www.rust-lang.org)

- [Crellvm](https://sf.snu.ac.kr/crellvm): a verified credible compilation framework for LLVM

- [SepCompCert](https://sf.snu.ac.kr/sepcompcert): verification of separate compilation of CompCert


#### Invited Talks

- iRRAM-Coq: Fearless Verification of Exact Real Arithmetic Programs.

  The 1st Workshop on Real Verification (RV 2017).

  \[[development](https://github.com/jeehoonkang/iRRAM-coq)\]


#### Awards and Honors

- Doctoral Dissertation Award, Dept. of Computer Science and Engineering, Seoul National University, 2019.

- Distinguished Paper Award, ACM SIGPLAN conference on Programming Languages Design and Implementation (PLDI), 2017.

<!-- - 23rd place, ACM International Collegiate Programming Contest (ICPC) World Finals, 2008. -->

<!-- - Champion, ACM International Collegiate Programming Contest (ICPC) Regional Contest---Seoul, 2007. -->

<!-- - Gold Medal, International Olympiad in Informatics (IOI), 2005. -->

#### Calendar

<div class="responsive-iframe-container big-container">
    <iframe src="https://calendar.google.com/calendar/embed?showTitle=0&amp;showPrint=0&amp;mode=WEEK&amp&amp;wkst=1&amp;bgcolor=%23FFFFFF&amp;src=jeehoon.kang%40cp.kaist.ac.kr&amp;color=%23125A12&amp;ctz=Asia%2FSeoul" style="border-width:0; margin-top:15pt;" frameborder="0" scrolling="no"></iframe>
</div>
<div class="responsive-iframe-container small-container" style="height: 1000;">
    <iframe src="https://calendar.google.com/calendar/embed?showTitle=0&amp;showPrint=0&amp;mode=AGENDA&amp&amp;wkst=1&amp;bgcolor=%23FFFFFF&amp;src=jeehoon.kang%40cp.kaist.ac.kr&amp;color=%23125A12&amp;ctz=Asia%2FSeoul" style="border-width:0" frameborder="0" scrolling="no"></iframe>
</div>
