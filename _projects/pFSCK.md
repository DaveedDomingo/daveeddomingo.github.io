---
layout: page
title: pFSCK
description: Accelerating File System Checking
img: /assets/projects/pFSCK/pFSCK-logo.png
---


<div class="img_row">
    <img class="col three left" src="{{ site.baseurl }}/assets/projects/pFSCK/pFSCK-banner.png" alt="" title="pFSCK banner"/>
</div>

### Introduction

Traditional file system checking has been notorious for being a tedious and long process making it a last resort for most sysadmins dealing with file system corruption.

Despite crash recovery and consistency mechanisms such as journaling being developed to mitigate the need to perform complete file system checking, file system checking is still the ultimate recovery tool when all other recovery techniques fail.

pFSCK, which is based on the e2fsck file system checker for EXT4 file systems, aims to explore the issues of traditional file system checking and attempts to automatically scale file system checking to exploit available multicore and storage parallelism to enable faster and more convenient file system checking.

You can read more about our project in our ArXiv pre-print here: [https://arxiv.org/abs/2004.05524](https://arxiv.org/abs/2004.05524)


### Papers and Presentations

1. Presented at [Linux Storage and Filesystems Conference (VAULT '20)](https://www.usenix.org/conference/vault20) as ["Accelerating Filesystem Checking and Repair with pFSCK"](https://www.usenix.org/conference/vault20/presentation/domingo)
2. ArXiv pre-print: [https://arxiv.org/abs/2004.05524](https://arxiv.org/abs/2004.05524)
