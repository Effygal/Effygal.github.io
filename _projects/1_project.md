---
layout: page
title: "TTL Approximations for a Family of CLOCK-Like Cache Replacement Policies"
description: "We extend TTL approximations to a family of CLOCK-like cache policies termed CLOCK($K$) and establish several structural properties of it: 1) CLOCK($K$) miss ratio is Schur-concave over frequency; b) the mean-field limit of CLOCK($K$) converges to its randomized counterpart Ran-CLOCK($K$) as $K$ tends to infinity." 
importance: 1
category: analytical modeling 
related_publications: 
---

## Abstract
We study a family of CLOCK-like policies, termed CLOCK($K$), which recovers FIFO at $K=0$ and classical second-chance CLOCK at $K=1$. Through a TTL-based approximation, we derive miss-ratio predictions for CLOCK($K$) across cache sizes under both Markovian and general renewal traffic. We validate these predictions using synthetic workloads and production traces, showing that the \emph{renewal traffic} model defined over coarse object classes, rather than per-object renewal processes, are sufficient to accurately capture CLOCK($K$) behavior beyond the memoryless regime. 

Our analysis further establishes structural properties of CLOCK($K$), including Schur-concavity of its miss probability in the popularity vector and convergence of CLOCK($K$) to its randomized counterpart Ran-CLOCK($K$) as $K$ grows large.
