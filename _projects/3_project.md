---
layout: page
title: "Fair Resource Allocation with Source-Side Throttling and FCFS Destination-Side Servicing"
description: "This project demonstrates a proof-of-concept approach for addressing performance isolation, QoS, and device capacity constraints in multi-tenant cloud environments using a unified linear programming model." 
importance: 1
category: distributed systems
related_publications: 
---

## Abstract
Performance isolation is essential but challenging in multi-tenant cloud storage systems. In private clouds such as vSAN, multiple virtual disks may be striped over the same physical device, causing congestions especially when some workloads experience bursts. 

We argue that an effective resource allocation mechanism should be lightweight, distributed, and non-intrusive, eliminating the need for a single bottleneck controller, or reliance on specialized device features. 

We propose a source-side hierarchical IOPS allocation design, scheduling per-VM I/Os using the hypervisor's throttling mechanism, while preserving the common FCFS servicing assumption at the physical devices. A unified linear programming formula is triggered in a feedback loop to solve for the optimal IOPS rate for each virtual disk, maximizing system throughput under QoS constraints and physical device capacities. 

Simulation demonstrates that this design effectively throttles I/O at an optimized rate, isolates burst traffic at the source, and significantly reduces congestion at the destination, thereby lowering overall end-to-end latency.

Available at [GitHub](https://github.com/Effygal/vm-qos).
