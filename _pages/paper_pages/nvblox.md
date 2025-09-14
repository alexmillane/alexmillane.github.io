---
permalink: /nvblox/
title: "nvblox"
excerpt: "nvblox"
author_profile: true
redirect_from: 
  - /nvblox.html
---

## Abstract

Dense, volumetric maps are essential to enable robot navigation and interaction with the environment. To achieve low latency, dense maps are typically computed onboard the robot, often on computationally constrained hardware. Previous works leave a gap between CPU-based systems for robotic mapping which, due to computation constraints, limit map resolution or scale, and GPU-based reconstruction systems which omit features that are critical to robotic path planning, such as computation of the Euclidean Signed Distance Field (ESDF). We introduce a library, nvblox, that aims to fill this gap, by GPU-accelerating robotic volumetric mapping. Nvblox delivers a significant performance improvement over the state of the art, achieving up to a 177x speed-up in surface reconstruction, and up to a 31x improvement in distance field computation, and is available open-source.

<!-- ## Materials -->

[code](https://github.com/nvidia-isaac/nvblox).
[paper](https://arxiv.org/pdf/2311.00626.pdf).
[docs](https://nvblox.gitlab-master-pages.nvidia.com/nvblox/)



## Paper
<!-- Ran: pdftoppm -png -r 60 nvblox_paper.pdf nvblox -->

[![nvblox](/files/nvblox/nvblox-1.png){:height="20%" width="20%"}
![nvblox](/files/nvblox/nvblox-2.png){:height="20%" width="20%"}
![nvblox](/files/nvblox/nvblox-3.png){:height="20%" width="20%"}
![nvblox](/files/nvblox/nvblox-4.png){:height="20%" width="20%"}
![nvblox](/files/nvblox/nvblox-5.png){:height="20%" width="20%"}
![nvblox](/files/nvblox/nvblox-6.png){:height="20%" width="20%"}
![nvblox](/files/nvblox/nvblox-7.png){:height="20%" width="20%"}](https://arxiv.org/pdf/2311.00626.pdf)

<!-- ## Video

[![Voxgraph](/images/voxgraph_video_thumbnail.jpeg)](https://www.youtube.com/watch?v=N9p1_Fkxxro){:target="_blank"} -->