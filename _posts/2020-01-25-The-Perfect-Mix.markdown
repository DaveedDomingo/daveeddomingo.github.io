---
layout: post
title: Finding the Perfect Remote Shell Setup
date: 2020-01-25 11:59:00-0400
description: Mosh + Tmux = Perfect Match
comments: true
---

For years i've been feeling like a super user; connected to remote computers via SSH, and using VIM to do development work on a remote system. My idea of multitasking on a remote system was by using multiple terminals, each with their own SSH connection to the system. I would further move back in forth between tasks within a single session by using ctrl+z to stop to and then bringing them back to the forward by using `fg`.

### Tmux: Goodbye Mouse and Window Borders
The moment I discovered TMUX I was in love. Due to previous trauma experienced when learning VIM, I was very hesitant on learning any other tool, thinking the learning curve would be the same. However, I was very surpised how easy it was to get a hang of Tmux.

You can create a new session:

```
$ tmux new -s <session name>
```

Detaching from the session is simply `CTRL+B` followed by `D` in quick succession.

You can then list the available sessions:
```
$ tmux ls
```
and attach to them using:
```
$ tmux attach -t <session name>
```
You can split the pane horizontally with `CTRL+B` followed by `%`. You can also split the pane vertically with `CTRL+B` followed by `"`. To move between the panes you just use `CTRL+B` followed by an arrow key specifying the direction in which to move. Moving and resizing windows you can the Tmux commands `swap-pane` and `resize-pane`, respectively. You can also create multiple windows in the same session, each with their own pane layout.

With Tmux I discovered what real remote shell multitasking is like. Being able to run multiple shells in parallel within the same window feels amazing as I do everything I need to do without taking my hand off the keyboard to click another window. Lastly, now I can completely avoid spending time resizing any windows with my mouse so they perfectly tile accross my desktop.

#### The Issue
Even though Tmux worked great, I was still left with the issue of spotty coffee shop WiFi which left me disconnected from time to time. When this happens, I have to restart the connection, then reattach to the Tmux session. Although this was such a little thing to do, it was still pretty annoying to have to do from time to time.

### Mosh:
Mosh is a remote terminal client that allows for intermittent connectivity by setting up a UDP connection between the client and the server via SSH. The Mosh server running in the background keeps any sessions alive in the event the client disconnects. Due to the connection, it allows the client to reconnect despite moving between networks or access points.

If you network goes down or your connection becomes spotty, Mosh will even show how long the connection was down for to let you know that you're connection, is indeed no working, so no need to double check if you can access the web from a web browser, when your session freezes and you think you may not have internet. 

#### The only downside: No X11 Forwarding
The only issue with Mosh is that X11 forwarding, which is a bummer as I like to run performance profiling applications such as Intel's VTune so I can see the performance graphs immediately instead of graphing them myself. Until then, I'll just use X11 forwarding in the lab where my WiFi isn't spotty.
