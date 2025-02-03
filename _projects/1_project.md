---
layout: page
title: Frequency and Recency Both Matter - How FIFO and CLOCK Performance Respond to Popularity Skewness
description: "We extend Che’s approximation to analyze CLOCK cache performance under both request models and address three key properties: (1) IRM always yields well-behaved, convex LRU miss ratio curves; (2) with a fixed inter-arrival time distribution, FIFO performs worse when item popularity is skewed; conversely, (3) CLOCK performs better when item popularity is skewed. We present formal proofs for these properties." 
thumbnail: assets/img/MarkovChain4States.pdf
importance: 1
category: work
related_publications: 
---

## Abstract
Consider two request streams that share the same inter-arrival time distribution: (a) an Independent Reference Model (IRM) traffic, where requests are selected i.i.d. from a skewed (e.g., Zipf-like) item frequency distribution. By construction, the inter-arrival times of such traffic naturally form a hyperexponential distribution. (b) A hyperexponential renewal traffic, constructed by re-sampling the inter-arrival times from the same IAT distribution of the IRM traffic, but assigning items uniformly.
We extend Che’s approximation to analyze CLOCK cache performance under both request models and address three key properties: (1) IRM always yields well-behaved, convex LRU miss ratio curves; (2) with a fixed inter-arrival time distribution, FIFO performs worse when item popularity is skewed; conversely, (3) CLOCK performs better when item popularity is skewed. We present formal proofs for these properties.

These results explain why CLOCK outperforms LRU on certain workloads and why FIFO outperforms RANDOM in real workloads. More importantly, they suggest that neither IRM alone nor renewal models alone are sufficient to model non-LRU/non-LFU cache performance. Both skewness in item popularity (frequency) and the IAT distribution are essential.

We propose a practical two-dimensional analytical model for real workload analysis, combining frequency- based workload decomposition with recency-based modeling for each substream. We demonstrate that this approach accurately predicts FIFO and CLOCK cache performance for real-world workloads from the CloudPhysics corpus.