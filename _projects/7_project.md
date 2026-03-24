---
layout: page
title: "Performance Analysis of the Randomized SIEVE/CLOCK Cache Replacement Algorithm (SIGMETRICS'26)"
description: "We introduce a randomized variant of the SIEVE/CLOCK algorithm that is scan-resistant, which uses only ⌈log2(K+1)⌉ ≥ 1 access bits per cached item, and we present a heterogeneous mean-field approximation of its performance." 
importance: 2
category: analytical modeling 
related_publications: 
---

## Abstract
Recently SIEVE was introduced as a new cache-eviction algorithm that excels in efficiency and simplicity. Like the CLOCK algorithm it uses a single list and an {\it access bit} per cached item. The SIEVE and CLOCK algorithm operate in the same manner, except that SIEVE inserts items in a fixed position in the list, instead of in the position of the evicted item. Both the SIEVE and CLOCK algorithm can be naturally generalized to a setting where multiple access bits are used per cached item.

Motivated by the need to improve the performance for workloads with long scan sequences, we introduce a randomized version of the SIEVE/CLOCK algorithm using $\lceil \log_2 (K+1) \rceil \geq 1$ access bits per cached item.  We present a heterogeneous mean-field model to assess the performance of the randomized SIEVE/CLOCK algorithm and prove that it has a unique fixed point that can be easily computed using bisection. An explicit expression for the fixed point is presented when $K$ tends to infinity. The accuracy of the model is demonstrated using simulations. Theoretical support for the observed accuracy is presented by arguing that the mean-field model of a slightly modified version of the algorithm is $O(1/n)$ accurate, where $n$ is the population size. 

We end the paper by comparing the performance of the randomized SIEVE/CLOCK algorithm with other cache replacement algorithms to demonstrate improved hit rates (by a factor $1.5$ or more) on workloads with long scan sequences. Furthermore, though the cache hit rate improves with the number of access bits, we show that the majority of the gain is already achieved with as few as $4$ access bits per cached item.
