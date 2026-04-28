---
layout: page
title: "A Cache-Accurate Storage Microbenchmark (EuroSys'26)"
description: "2DIO is a configurable I/O trace generator capable of producing cache-accurate workloads with tunable performance cliffs and plateaus." 
importance: 1
category: microbenchmarks
---

## Abstract
2DIO is a configurable I/O trace generator capable of producing cache-accurate workloads with tunable performance cliffs and plateaus. The framework encodes each workload as a compact parameter triplet that captures both short-term recency and long-term frequency, allowing systematic exploration of cache behaviors under different eviction policies. Parameters can be swept for explorative experimentation or calibrated to reproduce real-life hit ratio curves, enabling repeatable, scalable benchmarking.

Source code [GitHub](https://github.com/Effygal/trace-gen).