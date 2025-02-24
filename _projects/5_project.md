---
layout: page
title: "A simple cache simulator lib"
description: "We introduce an LRU 2C-array algorithm; it is an efficient method for implementing a cache eviction policy using a fixed-size array; it is particularly suitable for scenarios where memory constraints prevent the use of linked lists."
importance: 1
category: open-source
related_publications: 
---

## Abstract
We introduce an LRU 2C-array algorithm; it is an efficient method for implementing a cache eviction policy using a fixed-size array; it is particularly suitable for scenarios where memory constraints prevent the use of linked lists. 
```cpp
/*
  +-+-+-+-+-+-+-+-+-+-+-+-+-+
  | | |x| |x| |x| | | | | | |
  +-+-+-+-+-+-+-+-+-+-+-+-+-+
   0   ^         ^
	   |         head ->
	   tail ->
  head points to first unoccupied entry
  tail may point to empty entry
 */
```
- Instead of using a linked list, the algorithm keeps an array A of size 2C, where C represents the cache size.
- Array A stores items (e.g. pointers) in the cache and NULL values to indicate empty slots.
- Keeps a hash table H to store integer indexes of the items in A.
- 'head' points to the first unoccupied entry in A, and 'tail' points to the oldest item in A, might be NULL.

Available at [GitHub](https://github.com/Effygal/cachesim-cpp).

