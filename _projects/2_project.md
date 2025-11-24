---
layout: page
title: "Configurable and Cache-Accurate Trace Generation for Storage Benchmarking"
description: "2DIO is a configurable I/O trace generator capable of producing cache-accurate workloads with tunable performance cliffs and plateaus." 
importance: 1
category: open-source
related_publications: EuroSys'26
---

## Abstract
2DIO is a configurable I/O trace generator capable of producing cache-accurate workloads with tunable performance cliffs and plateaus. The framework encodes each workload as a compact parameter triplet that captures both short-term recency and long-term frequency, allowing systematic exploration of cache behaviors under different eviction policies. Parameters can be swept for explorative experimentation or calibrated to reproduce real-life hit ratio curves, enabling repeatable, scalable benchmarking.

Available at [GitHub](https://github.com/Effygal/trace-gen).