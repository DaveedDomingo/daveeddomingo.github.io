---
layout: page
title: CommandQueue
description: Easy Command and Batch Job Parallelism 
img: assets/img/commandqueue-logo.png
importance: 2
category: tools
related_publications: false
---

## Introduction
Sometimes you need run many commands and/or many batch jobs. Maybe you want to control how many commands/jobs are being ran at any particular time or maybe you also want to continually add to the queue of commands, modify queued commands, or even change order of commands to run.

*CommandQueue* is a job scheduling tool to run commands across all available cores and limits simultanous execution to avoid unessecary multiplexing. You can programatically modify the queue of commands to run or simply use your favorite text editor. Written as a python script that runs in the background, it is cross compatible across Windows, Mac, and Linux.


##### Features:
1. **Configurable Core Count.** User can specify the amount of processes to use to control parallelism
2. **Easy to use.** Simply add/modify/reorder the command queue with your favorite text editor
3. **Cross-Compatible.** Works on Windows, Mac, and Linux.


##### How to Use: 
See documentation on how to use CommandQueue at the GitHub link below.


**Github Link:** [https://github.com/DaveedDomingo/CommandQueue](https://github.com/DaveedDomingo/CommandQueue)


<br />

------------


## Back Story:
During a research project, I needed to run simulations for various system design configurations over large amounts of data traces. Each simulation could take minutes to up to hours based on the size of the trace and unfortunately the simulator I built was single threaded due to the need for event serialization to enable determinism and fine grained introspection between any two events that may occur within the distributed system I was simulating. 

To ensure simulation throughput and make use of all available cores, I needed to run multiple simulations at the same time, but I wasn't happy with available job scheduling tools. From what I could see, there weren't any simple tools that allowed me to queue up commands/jobs and limit the amount of commands running any time so I don't unecessarily multiplex the CPUs available. Additionally I wanted to make a queue of commands that I can easily edit, and have the job scheduler simply pick up the next command on the queue to ensure no idle time as long as there's commands to run.

So I decided to make CommandQueue. This tool made me feel at ease making me know all commands would be executed efficiently across all CPUs. I could queue up large amounts of simulations to run over the weekend and check up on the results on Monday. Additionally, since I could easily modify the queue using a texteditor, if there were some interesting insights from finished simulations, I could easily add additional commands to simulate additional (potentially interesting) system configurations at the end of the queue (or even at the front of the queue if I reallt felt it would yield some interesting results). Overall i'm happy I made this tool and still use this tool to this day. I wrote it in Python so I can use it in any environment I may be using.  




