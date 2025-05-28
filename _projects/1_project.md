---
layout: page
title: "Properties of FIFO and CLOCK cache under general renewal traffic"
description: "We extend Che’s approximation to the canonical second-chance CLOCK under general renewal traffic and formally prove two properties: (1) LRU miss rate is convex over cache size under IRM; (2) CLOCK’s miss rate is Schur-concave over request rates." 
importance: 1
category: analytical modeling 
related_publications: 
---

## Abstract
We present exact analyses of cache performance under renewal traffic models that isolate frequency skew from temporal locality. Focusing on FIFO and a family of CLOCK caches with reference bits, we derive exact miss rate expressions and validate them against both synthetic workloads (MAE < 0.3\%) and production block‐storage traces (MAE < 2.3\%). 
  
A common belief is that while CLOCK respects recency, it does not take frequency into account. Our main theorem challenges this belief, extend those of van den Berg and Towsley (1993), showing that CLOCK’s miss rate is Schur-concave over the request rate vector. Several properties then emerge: with temporal locality held fixed, increasing frequency skew degrades FIFO performance but enhances CLOCK’s performance, thereby explaining why CLOCK can outperform LRU and why FIFO often outperforms RANDOM in practice.
<!-- ![](../clock-levels.webp) -->