---
layout: people
title: Concurrent Garbage Collectors
description: Garbage in, garbage out
background: /assets/images/kaist.jpg
permalink: /gc
---


> To collect or not to collect, that is the garbage question.
> <br />
> ---Unknown

All pointer-based nonblocking concurrent data structures should deal with the problem of <em>safe
memory reclamation</em>: before reclaiming a memory block, a thread should make sure that no other
threads are concurrently dereferencing the block.  Various safe memory reclamation schemes have been
proposed in the literature, but none of them is clearly better than the others in every aspect.  The
trade-offs indicate the complex nature of memory reclamation.

We aim to break the trade-offs by combining the great ideas of prior work and our new ideas in an
interesting way, producing the off-the-shelf solution for safe memory reclamation.


### Publications

{% include publications.md tag="gc" submitted=true full=true %}
