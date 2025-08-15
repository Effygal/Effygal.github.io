---
layout: page
title: "How FIFO and CLOCK respond to ferquency skew"
description: "We extend van den Berg and Toswley’s proof of the Schur-convexity of FIFO miss ratio to explain why FIFO out-performs RANDOM on real workloads, while using our proofs to explain why CLOCK often out-performs LRU." 
importance: 1
category: analytical modeling 
related_publications: 
---

## Abstract
The performance of non-LRU or LFU caches is affected by both frequency and recency, but while prior work on replacement policies has treated these factors intuitively, analytic models have not delved deeply into their separate roles. We present a framework to isolate
the effects of each dimension, allowing explicit derivation of miss ratio formulas as frequency and recency are varied, and validate our
models in simulation, with mean absolute error for FIFO and CLOCK of < 0.3\% for synthetic workloads and < 2.3\% for production block storage traces.
Our main theorem shows that the CLOCK miss ratio function is Schur-concave in the frequency vector; for fixed recency distribution, miss ratio decreases with increasing frequency skew. Real workloads are not purely IRM, yet contain significant frequency skew; we extend van den Berg and Toswley’s proof of the Schur-convexity of FIFO miss ratio to explain why FIFO out-performs RANDOM on real workloads, while using our proofs to explain why CLOCK often out-performs LRU.
<!-- ![](../clock-levels.webp) -->