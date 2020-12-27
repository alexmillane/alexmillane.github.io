---
permalink: /cblox/
title: "Cblox"
excerpt: "Cblox"
author_profile: true
redirect_from: 
  - /cblox.html
---

## Abstract

In many applications, maintaining a consistent dense map of the environment is key to enabling robotic platforms to perform higher level decision making. Several works have addressed the challenge of creating precise dense 3D maps from visual sensors providing depth information. However, during operation over longer missions, reconstructions can easily become inconsistent due to accumulated camera tracking error and delayed loop closure. Without explicitly addressing the problem of map consistency, recovery from such distortions tends to be difficult. We present a novel system for dense 3D mapping which addresses the challenge of building consistent maps while dealing with scalability. Central to our approach is the representation of the environment as a collection of overlapping TSDF subvolumes. These subvolumes are localized through feature-based camera tracking and bundle adjustment. Our main contribution is a pipeline for identifying stable regions in the map, and to fuse the contributing subvolumes. This approach allows us to reduce map growth while still maintaining consistency. We demonstrate the proposed system on a publicly available dataset and simulation engine, and demonstrate the efficacy of the proposed approach for building consistent and scalable maps. Finally we demonstrate our approach running in real-time on-board a lightweight MAV.

<!-- ## Materials -->

[code](https://github.com/ethz-asl/cblox).
[paper](https://arxiv.org/pdf/1710.07242.pdf).
<!-- [video](https://www.youtube.com/watch?v=N9p1_Fkxxro). -->



## Paper

[![Cblox](/files/cblox/cblox-0.png){:height="20%" width="20%"}
![Cblox](/files/cblox/cblox-1.png){:height="20%" width="20%"}
![Cblox](/files/cblox/cblox-2.png){:height="20%" width="20%"}
![Cblox](/files/cblox/cblox-3.png){:height="20%" width="20%"}
![Cblox](/files/cblox/cblox-4.png){:height="20%" width="20%"}
![Cblox](/files/cblox/cblox-5.png){:height="20%" width="20%"}
![Cblox](/files/cblox/cblox-6.png){:height="20%" width="20%"}
![Cblox](/files/cblox/cblox-7.png){:height="20%" width="20%"}](https://arxiv.org/pdf/1710.07242.pdf)

<!-- ## Video

[![Voxgraph](/images/voxgraph_video_thumbnail.jpeg)](https://www.youtube.com/watch?v=N9p1_Fkxxro){:target="_blank"} -->