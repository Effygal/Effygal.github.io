---
layout: page
title: "Dynamic Hierarchical Throttling for vSAN"
description: "This project focuses on resource allocation in VMware vSAN using a dynamic linear programming model
to optimize traffic across virtual and physical resources while adhering to SLA constraints. Instead of
relying on a centralized controller, it leverages VM hypervisor capabilities to reduce queue delays. The
approach also implements multi-hierarchical token control to enhance performance and fairness." 
thumbnail: assets/img/MarkovChain4States.pdf
importance: 1
category: work
related_publications: 
---

## Abstract
Multi-tenant cloud storage systems face performance interference from concurrent workloads. This project introduces a dynamic linear programming model for VMware's vSAN architecture. Instead of relying on a centralized controller, it implements throttling logic within hypervisors. The model uses hierarchical token buckets to regulate IOPS at multiple levels, while adherence to service-level limits. By dynamically allocating resources across shared physical disks, it minimizes queue delays and enhances fairness.