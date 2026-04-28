---
layout: page
title: "TTL Approximations for a Family of CLOCK-Like Cache Replacement Policies"
description: "We extend TTL-approximations to a family of CLOCK-like cache policies termed CLOCK(K), deriving a tractable matrix-analytic solution for steady-state miss ratios under phase-type renewal processes and establishing a Schur-concavity property of CLOCK(K=0)/FIFO." 
importance: 1
category: analytical modeling 
related_publications: 
---

## Abstract
Analytical miss-ratio modeling for CLOCK-like policies remains difficult, as the scan-based eviction path inherently couples object states and obscures the steady-state structure.

This work addresses this gap by analyzing a family of eviction policies, termed CLOCK($K$)~\cite{ran-clock} in which FIFO corresponds to $K=0$, the canonical CLOCK~\cite{corbato_paging_1968} corresponds to $K=1$. Concretely, we derive a time-to-live (TTL) approximation that decouples individual object dynamics using a global fixed timer. While this global TTL acts as a proxy for the physical cache capacity constraint, the resulting framework yields a tractable matrix-analytic solution for steady-state miss ratios under phase-type renewal processes, effectively reducing the problem to solving a per-object linear system of order $O(Kd)$, where $d$ is the phase dimension. The accuracy of the model is validated against trace-driven simulations. We further establish a Schur-concavity property of CLOCK($K=0$)/FIFO under this TTL-approximation, along with a necessary correction to a classical theorem of FIFO Schur-convexity in {% cite van1993properties %}.
