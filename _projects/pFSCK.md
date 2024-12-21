---
layout: page
title: pFSCK
description: Accelerating File System Checking for Modern Storage
img: assets/img/pFSCK-logo-square.jpg
importance: 1
category: work
related_publications: false
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/pFSCK-banner-long.jpg" title="pFSCK-banner" %}
    </div>
</div>

<br />

## Introduction
Traditional file system checking has been notorious for being a tedious and long process making it a last resort for most sysadmins dealing with file system corruption.

Despite crash recovery and consistency mechanisms such as journaling being developed to mitigate the need to perform complete file system checking, file system checking is still the ultimate recovery tool when all other recovery techniques fail.

pFSCK, which is based on the e2fsck file system checker for EXT4 file systems, aims to explore the issues of traditional file system checking and attempts to automatically scale file system checking to exploit available multicore and storage parallelism to enable faster and more convenient file system checking.

You can learn more here: [https://www.usenix.org/conference/fast21/presentation/domingo](https://www.usenix.org/conference/fast21/presentation/domingo)

Feel free to also check out our source code here: [https://github.com/RutgersCSSystems/pFSCK](https://github.com/RutgersCSSystems/pFSCK)

<br />

## Papers and Presentations
1. Appeared in [USENIX Conference on File and Storage Technologies (FAST ‘21)](https://www.usenix.org/conference/fast21) as ["pFSCK: Accelerating File System Checking and Repair for Modern Storage"](https://www.usenix.org/conference/fast21/presentation/domingo)
2. Presented at [Linux Storage and Filesystems Conference (VAULT ‘20)](https://www.usenix.org/conference/vault20) as [“Accelerating Filesystem Checking and Repair with pFSCK”](https://www.usenix.org/conference/vault20/presentation/domingo)