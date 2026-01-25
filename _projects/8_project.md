---
layout: page
title: "Performance Analysis of the Randomized SIEVE/CLOCK Cache Replacement Algorithm"
description: We introduce a randomized version of the SIEVE/CLOCK algorithm that uses ⌈log2(K+1)⌉ ≥ 1 access bits per cached item, and present a heterogeneous mean-field approximation of its performance." 
importance: 2
category: analytical modeling 
related_publications: 
---

## Abstract
Motivated by the need to improve the performance for workloads with long scan sequences, we introduce
a randomized version of the SIEVE/CLOCK algorithm using ⌈log2 (𝐾+1)⌉≥1 access bits per cached item.
We present a heterogeneous MF model to assess the performance of the randomized SIEVE/CLOCK
algorithm and prove that it has a unique fixed point that can be easily computed using bisection. An explicit expression for the fixed point is presented when 𝐾 tends to infinity. The accuracy of the model is validated against simulations. Theoretical support for the observed accuracy is presented by arguing that the MF model of a slightly modified version of the algorithm is 𝑂(1/𝑛) accurate, where 𝑛 is the population size.
