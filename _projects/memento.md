---
layout: people
title: Practical Detectability for Persistent Lock-Free Data Structures
description: Practical programming framework for persistent lock-free DSs with detectability
background: /assets/images/kaist.jpg
permalink: /memento
---

Persistent memory (PM) is an emerging class of storage technology
that combines the benefits of DRAM and SSD. This characteristic
inspires research on persistent objects in PM with fine-grained
concurrency control. Among such objects, persistent lock-free data
structures (DSs) are particularly interesting thanks to their efficiency and scalability. One of the most widely used correctness criteria for persistent lock-free DSs is *durable linearizability* (Izraelevitz
et. al., DISC 2016). However, durable linearizability is insufficient to
use persistent DSs for fault-tolerant systems requiring exactly-once
semantics for storage systems, because we may not be able to detect
whether an operation is performed when a crash occurs.

We present a practical programming framework for persistent
lock-free DSs with detectability. In contrast to the prior work on
such DSs, our framework supports

1. primitive detectable operations such as space-efficient compare-and-swap, insertion, and deletion;
1. systematic transformation of lock-free DSs in DRAM into those in PM requiring modest efforts;
1. comparable performance with non-detectable DSs by DRAM scratchpad optimization; and
1. recovery from both full system and thread crashes.

The key idea is *memento* objects serving as a lightweight, precise, and
per-thread checkpoints in PM. As a case study, we implement lockfree and combining queues and hash tables with detectability that
outperform (and perform comparably) the state-of-the-art DSs with
(and without, respectively) detectability.

### For VLDB 2022 reviewers

Here is an artifact zip file for your reivew: **[artifact.zip](https://drive.google.com/file/d/1S2sZW4Mf27wYHiGFD0y8KnWb4s6-q7IZ/view?usp=sharing)**

### Publications

{% include publications.md tag="memento" submitted=true abstract=true %}
