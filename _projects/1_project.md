---
layout: page
title: "TTL Approximations for CLOCK(K) Cache Replacement"
description: "We extend TTL approximations to a family of CLOCK-like cache policies termed CLOCK(K), deriving a tractable matrix-analytic solution for steady-state miss ratios under phase-type renewal processes." 
importance: 1
category: analytical modeling 
related_publications: 
---

## Abstract
While CLOCK-like cache replacement policies are highly appealing in practice due to their frugal memory usage and implementation simplicity, analytical models for their performance remain limited.
The difficulty stems from the "eviction hand" itself. As it scans sequentially for an evictee, sparing objects with survival counters along the way, it inherently entangles the state of one cached object with the next. This strong coupling heavily obscures the system's steady state.
  
To address this gap, we introduce a time-to-live (TTL) approximation for a family of eviction policies---which we term CLOCK($K$)---that decouples individual object dynamics using a globally fixed timer. In contrast to the intrinsic coupling induced by assuming a fixed cache capacity, such a TTL proxy yields a tractable matrix-analytic solution for the steady-state miss ratio functions across a broad and highly expressive class of phase-type renewal traffic. Among other benefits, this effectively reduces the analysis per-object to solving a linear system of order $O(Kd)$, where $d$ is the phase dimension. Moreover, our model for CLOCK($K$) recovers the canonical CLOCK when $K=1$ and FIFO when $K=0$, while exhibiting Schur-concavity empirically. Finally, we validate the model against a suite of trace-driven simulations. 
