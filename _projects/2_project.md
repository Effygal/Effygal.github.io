---
layout: page
title: "Configurable and Cache-Accurate Trace Generation for Storage Benchmarking"
description: "2DIO is a trace generator creating cache-accurate and stressful I/O workloads. While existing tools are limited to generating traces with well-behaved, concave hit ratio curves, 2DIO produces ones with tunable complex cache behaviors, particularly performance cliffs and plateaus." 
importance: 1
category: open-source
related_publications: EuroSys'26
---

## Abstract
We present 2DIO, a trace generator creating cache-accurate
        stressful I/O workloads. While existing tools are limited to
        generating traces with well-behaved, concave hit ratio curves,
        2DIO produces ones with tunable complex cache behaviors,
        particularly performance cliffs and plateaus.
        
        Our framework encodes a workload as a compact parameter triplet, capturing both short-term recency and long-term frequency. This parsimonious parameterization allows researchers to easily translate individual adjustments into predictable cache effects across various eviction policies. It enables the parameter space to be "swept" for exhaustive exploration of desired cache behavior, or to mimic real traces by calibrating parameters to match observed behaviors. 

        The tuned parameters are portable, meaning if the scale of the system under evaluation changes, so too will the footprint and length of the trace, while the relative cache behaviors are preserved.
        
        Evaluations demonstrate 2DIO’s ability to customize traces
        with a continuum of "what-if" cache behaviors and to reproduce real-world ones with high accuracy.

Available at [GitHub](https://github.com/Effygal/trace-gen).