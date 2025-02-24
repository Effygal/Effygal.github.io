---
layout: page
title: "A Distributed Object Store built on Conventional File System"
description: "This is an emulation of a distributed store system built on Zoned Namespace SSDs. The system guarantees strong consistency and fault tolerant."
thumbnail: 
importance: 2
category: distributed systems
related_publications: 
---

## Abstract
FilelogKV is a distributed object storage system built on top of conventional file systems. It provides strong consistency and fault tolerance. It is an emulation of a distributed KV storage system which assumes the underlying storage devices are Zoned Namespace SSDs, whereby a "Zone Append" write semantic is used instead of conventional SSDs that depend on a flash translation layer. 
This project is suspended; currently works fine with below features:
* Accept PUT/GET/DELETE requests; functions as a conventional KV storage system.
* Failure tolerant as long as one gateway and one storage node are alive.
* Strong consistency: aggressive crash recovery assuming the recovery manager does not fail during recovery.
* Gateway nodes are scalable.

Available at [GitHub](https://github.com/Effygal/zns-obj/tree/main/Filelog-KV).

