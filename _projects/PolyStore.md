---
layout: page
title: PolyStore
description: Exploiting Combined Capabilities of Heterogeneous Storage
img: assets/img/polystore-logo.png
importance: 2
category: research
related_publications: false
---

## Introduction
Advancements in computer storage has led to a large variety of devices that provide significant bandwidth capabilities at low latencies. These advancements has led to an increase in hetergenous storage systems as consumers adopt these new technologies into their current setups.

Traditional heterogenous storage management approaches take a heirarchal approach, placing the faster, more performant device on top of the slower device. The faster device is used as either a cache, or as a place for fast data staging, and data is then moved between the fast and slow device to adjust to data access patterns and data hotness. However, these approaches fail to realize the potential performance across the devices as data flow is resticted to a single path through the fast device. This effectively limits potential performance to that of the fast device.

PolyStore, built as a meta-layer library, aims to explore how to extract performance across hetergenous storage by taking a non-heirachical approach, enabling the ability to split file data across devices and flexibly use both storage devices simultanously.

You can learn more here: [https://www.usenix.org/conference/fast25/presentation/ren](https://www.usenix.org/conference/fast25/presentation/ren)

Feel free to also check out our source code here: [https://github.com/RutgersCSSystems/PolyStore](https://github.com/RutgersCSSystems/PolyStore)

<br />

## Papers and Presentations
1. Appeared in [USENIX Conference on File and Storage Technologies (FAST ‘25)](https://www.usenix.org/conference/fast25) as ["PolyStore: Exploiting Combined Capabilities of Heterogeneous Storage"](https://www.usenix.org/conference/fast25/presentation/ren)