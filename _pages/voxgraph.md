---
permalink: /publications/
title: "Voxgraph"
excerpt: "Voxgraph"
author_profile: true
redirect_from: 
  - /voxgraph/
  - /voxgraph.html
---

## Abstract

Globally consistent dense maps are a key requirement for long-term robot navigation in complex environments. While previous works have addressed the challenges of dense mapping and global consistency, most require more computational resources than may be available on-board small robots. We propose a framework that creates globally consistent volumetric maps on a CPU and is lightweight enough to run on computationally constrained platforms. Our approach represents the environment as a collection of overlapping Signed Distance Function (SDF) submaps, and maintains global consistency by computing an optimal alignment of the submap collection. By exploiting the underlying SDF representation, we generate correspondence free constraints between submap pairs that are computationally efficient enough to optimize the global problem each time a new submap is added. We deploy the proposed system on a hexacopter Micro Aerial Vehicle (MAV) with an Intel i7-8650U CPU in two realistic scenarios: mapping a large-scale area using a 3D LiDAR, and mapping an industrial space using an RGB-D camera. In the large-scale outdoor experiments, the system optimizes a 120x80m map in less than 4s and produces absolute trajectory RMSEs of less than 1m over 400m trajectories. Our complete system, called voxgraph, is available as open source.

## Paper

[![Freetures](/files/voxgraph/voxgraph-0.png){:height="20%" width="20%"}
![Freetures](/files/voxgraph/voxgraph-1.png){:height="20%" width="20%"}
![Freetures](/files/voxgraph/voxgraph-2.png){:height="20%" width="20%"}
![Freetures](/files/voxgraph/voxgraph-3.png){:height="20%" width="20%"}
![Freetures](/files/voxgraph/voxgraph-4.png){:height="20%" width="20%"}
![Freetures](/files/voxgraph/voxgraph-5.png){:height="20%" width="20%"}
![Freetures](/files/voxgraph/voxgraph-6.png){:height="20%" width="20%"}
![Freetures](/files/voxgraph/voxgraph-7.png){:height="20%" width="20%"}](https://arxiv.org/pdf/2004.13154.pdf)