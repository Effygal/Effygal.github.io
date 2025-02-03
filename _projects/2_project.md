---
layout: page
title: "Configurable and Cache-Accurate Trace Generation for Storage Benchmarking"
description: "We introduce 2DIO, a two- dimensional trace generation framework that encodes cache behaviors through a compact, quantized representation of recency patterns (IRD), combined with an independent reference model that characterizes frequency. This approach requires minimal parameters yet accurately reproduces complex, non-convex LRU miss ratio curves observed in real workloads." 
thumbnail: assets/img/MarkovChain4States.pdf
importance: 1
category: work
related_publications: 
---

## Abstract
We address two observed patterns in real-world storage I/O traces: (1) their inter-arrival distance (IRD) distributions show multiple cliffs and plateaus in the short term and converge to heavy-tailed distributions in the long term; (2) the cliffs (or plateaus) in their LRU miss ratio curve correspond to the spikes (or holes) in their IRD distribution.
Based on these observations, we introduce 2DIO, a two- dimensional trace generation framework that encodes cache behaviors through a compact, quantized representation of re- cency patterns (IRD), combined with an independent reference model that characterizes frequency. This approach requires minimal parameters yet accurately reproduces complex, non-convex LRU miss ratio curves observed in real workloads.
Our evaluation compares 2DIO to state-of-the-art methods, including deep learning approaches, demonstrating its cache accuracy and low cost. 2DIO scales with trace length and footprint while providing flexible configuration to replicate or customize a wide range of LRU miss ratio behaviors.