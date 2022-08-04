---
title: Thread-safe Malloc Library
date: 2022-08-04T16:19:12.378Z
summary: "*• Implemented malloc library in C based on First Fit and Best Fit
  strategies, which features merging/splitting adjacent free regions*"
draft: false
featured: false
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
*• Implemented malloc library in C based on First Fit and Best Fit strategies, which features merging/splitting*

*adjacent free regions*

*• Enabled thread-safe with the implementation of lock and lock-free versions using mutex synch strategy and*

*thread-local storage to prevent race conditions*

*• Handle 1 billion memory allocation and deallocation within 60 seconds in both First Fit and Best Fit strategies*