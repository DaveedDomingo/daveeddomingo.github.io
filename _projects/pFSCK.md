---
layout: page
title: pFSCK
description: Accelerating File System Checking
img: /assets/projects/pFSCK/pFSCK-logo.png
---


### Introduction

Traditional file system checking has been notorious for being a tedious and long process making it a last resort for most sysadmins dealing with file system corruption.

Despite crash recovery and consistency mechanisms being developed to mitigate the need to perform complete file system checking, file system checking is still the ultimate recovery tool when all other recovery techniques fail.

pFSCK aims to explore the issues of traditional file system checking and attempts to exploit available multicore and storage parallelism to enable faster and more convenient file system checking.

Based of e2fsck file system checker for EXT4.

This work is still ongoing with plans to ensure exploring new ways to carry out file system checking

You can read more about our project in our ArXiv preprint here: [https://arxiv.org/abs/2004.05524](https://arxiv.org/abs/2004.05524)

### Papers and Presentations

1. Presented at [Linux Storage and Filesystems Conference (VAULT '20)](https://www.usenix.org/conference/vault20) as ["Accelerating Filesystem Checking and Repair with pFSCK"](https://www.usenix.org/conference/vault20/presentation/domingo)
2. ArXiv preprint: [https://arxiv.org/abs/2004.05524](https://arxiv.org/abs/2004.05524)
