---
layout: page
title: "A TTL-Based Analysis of Counter-Driven Circular Cache Replacement"
description: "We extend TTL-approximations to a family of CLOCK-like cache policies termed CLOCK(K), deriving a tractable matrix-analytic solution for steady-state miss ratios under phase-type renewal processes and establishing a Schur-concavity property of CLOCK(K=0)/FIFO." 
importance: 1
category: analytical modeling 
related_publications: 
---

## Abstract
While CLOCK-like cache replacement policies are highly appealing in practice due to their frugal memory usage and implementation simplicity, analytically modeling their performance remains a challenge. The core issue stems from the recycling mechanism of their "eviction hand". By granting cached objects one or more chances to survive from evictions, this mechanism inherently couples object states and heavily obscures the steady-state of the system. To address this gap, we introduce a time-to-live (TTL) approximation for a family of eviction policies---which we term CLOCK($K$)---that decouples individual object dynamics using a global fixed timer. In contrast to the intrinsic coupling induced by assuming a fixed cache capacity, such a TTL proxy yields a tractable matrix-analytic solution for the steady-state miss ratios across a broad and highly expressive class of phase-type renewal traffic. Among other benefits, this effectively reduces the analysis of per-object miss ratios to solving a linear system of order $O(Kd)$, where $d$ is the phase dimension. Moreover, our model for CLOCK($K$) recovers the canonical CLOCK when $K=1$, and the classical FIFO when $K=0$, wherein it exhibits Schur-concavity under a globally fixed TTL. Finally, we validate the accuracy of the model against a suite of trace-driven simulations. 
