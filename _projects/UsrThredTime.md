---
layout: page
title: /usr/thread/time
description: "/usr/bin/time but for threads"
img: assets/img/usrthreadtime-logo.png
importance: 3
category: tools
related_publications: false
---


## Introduction
/usr/bin/time is such as useful tool as it can give you information about page faults, block reads, and context switches for a particular process. However, the default program only gives infomation about the whole process but sometimes you may want to get this kind of information at a thread granularity.

*Thread-Time* is a simple shim library to do just that. It simply has the same logic of /usr/bin/time, but does prints out out information on a per thread basis.

##### How to Use: 
See documentation on how to use thread-time at the GitHub link below.

**Github Link:** [https://github.com/DaveedDomingo/thread-time](https://github.com/DaveedDomingo/thread-time)

