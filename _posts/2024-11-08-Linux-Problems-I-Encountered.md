---
layout: post
title: "Linux Problems I Encountered"
author: "Fatin"
tags: Linux
excerpt_separator: <!--more-->
---

I write this to document my Linux journey, including some of the problems I've encountered and the solutions I've found.I will update this blog regularly.

## Clash Permissions Issue on Ubuntu 22.04

On Ubuntu 22.04, I'm not sure what I did, but it seems like I installed some dependencies, similar to those required by Wine. After that, Clash stopped working, but Shadowsocks was still functional. After confirming that it wasn't a port issue, I did some research and discovered that the problem was caused by insufficient permissions for Clash.
Finally, I opened Bash and added the following:

```
Exec=sudo /path/to/clash
```
