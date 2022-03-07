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

### For VLDB 2022 Reviewers

Here is an artifact zip file for your reivew: **[artifact.zip](https://drive.google.com/file/d/1S2sZW4Mf27wYHiGFD0y8KnWb4s6-q7IZ/view?usp=sharing)**

### Evaluaton Results

#### Queue

![queue-legend1](assets/images/paper/memento/queue-legend1.svg)
![queue-legend2](assets/images/paper/memento/queue-legend2.svg)

##### Multi-threaded Throughput of enqueue-dequeue pair
![queue-throughput-pair](assets/images/paper/memento/queue-throughput-pair.svg)

##### Multi-threaded Throughput of enqueue 20%, dequeue 80%
![queue-throughput-prob20](assets/images/paper/memento/queue-throughput-prob20.svg)

##### Multi-threaded Throughput of enqueue 50%, dequeue 50%
![queue-throughput-prob50](assets/images/paper/memento/queue-throughput-prob50.svg)

##### Multi-threaded Throughput of enqueue 80%, dequeue 20%
![queue-throughput-prob80](assets/images/paper/memento/queue-throughput-prob80.svg)


#### Hash Table

![hash-legend1](assets/images/paper/memento/hash-legend1.svg)
![hash-legend2](assets/images/paper/memento/hash-legend2.svg)

##### Tail Latency of Hash Tables with 32 Threads
![hash-latency](assets/images/paper/memento/hash-latency-multi32-uniform.svg)

##### Single-threaded Throughput of Hash Tables
![hash-single](assets/images/paper/memento/hash-throughput-single.svg)

##### Multi-threaded Throughput of Hash Tables for Self Similar Distribution with Factor 0.2
![hash-self1](assets/images/paper/memento/hash-throughput-multi-self-similar-0.2_1.svg)
![hash-self2](assets/images/paper/memento/hash-throughput-multi-self-similar-0.2_2.svg)

##### Multi-threaded Throughput of Hash Tables for Uniform Distribution
![hash-uniform1](assets/images/paper/memento/hash-throughput-multi-uniform1.svg)
![hash-uniform2](assets/images/paper/memento/hash-throughput-multi-uniform2.svg)

### Publications

{% include publications.md tag="memento" submitted=true abstract=true %}
