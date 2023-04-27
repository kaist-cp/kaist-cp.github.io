---
layout: people
title: Persistent Memory
description: The emerging class of storages between DRAM and SSD
background: /assets/images/kaist.jpg
permalink: /pmem
redirect_from:
  - /memento/
---


> Persísto, ergo sum.
> <br />
> ---Unknown

[Persistent memory](https://docs.pmem.io/persistent-memory/) is an emerging class of storage technology
that simultaneously provides (1) byte addressability, low latency, and high throughput as DRAM does;
and (2) durability (data persistency across system crashes) and high capacity as SSD does. These
powerful properties, however, have brought about existing issues such as (1) concurrency control for
thread safety and (2) persistency control for data consistency.

We aim to understand how to properly use this attractive memory in a program. In addition, we aim to
exploit its potentiality to build innovative transational systems!

### Publications

{% include publications.md tag="pmem" submitted=true abstract=true %}
