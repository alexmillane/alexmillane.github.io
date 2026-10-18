---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi, I’m Alex. I’m a tech-lead working on robotics at NVIDIA.

My work at NVIDIA has been at the intersection of real-time perception, robot learning, and simulation.
I have a PhD in computer vision and robotics from ETH Zurich where I studied in the Autonomous Systems Lab (ASL) under Roland Siegwart.

I love working with passionate small teams on hard problems that lie at the intersection of mathematics, software, and physical systems.


## Work at Nvidia
Open-source things that I've worked on at NVIDIA.

{% capture weaverl-text %}
<div class="project-card">
  <div class="project-card__media">
    <p>
      <a href="https://weave-rl.github.io/" title="WeaveRL project page">
        <video width="300" autoplay loop muted playsinline preload="metadata" poster="/images/weaverl_composite.jpg" aria-label="WeaveRL: real-robot shelf placement on the left, parallel simulated environments and their 3D reconstructions on the right" style="display: block;">
          <source src="/images/weaverl_composite.mp4" type="video/mp4">
        </video>
      </a>
    </p>
  </div>
  <div class="project-card__text">
    <h2 style="margin-top: 0;">3D Reconstruction for Reinforcement Learning</h2>
    <p>
    We bring online 3D reconstruction into massively parallel reinforcement learning, allowing robots to learn manipulation skills in geometrically complex scenes.
    Our GPU-accelerated system reconstructs thousands of simulated environments in parallel and uses that geometry to guide collision avoidance.
    </p>
    <p>
    Our approach allows completion of collision-dense tasks that map-free approaches fail at.
    Furthermore, these policies transfer sim to real zero shot, and show increased robustness to unseen obstacles.
    </p>
    <p>
    Check out the <a href="https://weave-rl.github.io/" title="WeaveRL project page">project page</a> and
    <a href="https://arxiv.org/abs/2609.18685" title="WeaveRL paper">paper</a>.
    </p>
  </div>
</div>
{% endcapture %}

<div class="notice--primary" style="float: left">
  {{ weaverl-text | markdownify }}
</div>

{% capture arena-text %}
<div class="project-card">
  <div class="project-card__media">
    <p>
      <video width="300" autoplay loop muted playsinline style="display: block;">
        <source src="/images/arena_parallel_evaluation.mp4" type="video/mp4">
      </video>
    </p>
  </div>
  <div class="project-card__text">
    <h2 style="margin-top: 0;">Isaac Lab Arena</h2>
    <p>
    Parallel simulation for robot policy evaluation at scale.
    Arena provides tools for scalable simulation environment generation.
    For example one can place objects automatically from semantic
    spatial relationships.
    Simulation environments can be co-designed with an agent.
    We exploit parallelism at multiple levels for fast evaluation, multiple simulation environments per GPU, and multi-node execution on GPU compute clusters.
    </p>
    <p>
    Check out the <a href="https://isaac-sim.github.io/IsaacLab-Arena/main/index.html" title="Isaac Lab Arena documentation">documentation</a> and
    <a href="https://github.com/isaac-sim/IsaacLab-Arena/" title="Isaac Lab Arena code">code</a>.
    </p>
  </div>
</div>
{% endcapture %}

<div class="notice--primary" style="float: left">
  {{ arena-text | markdownify }}
</div>


{% capture mindmap-text-2 %}
<div class="project-card">
  <div class="project-card__media">
    <p>
      <img src="/images/mindmap_robot.png" alt="humanoid robot in IsaacLab" width="300" style="display: block; margin-bottom: 10px;"/>
      <img src="/images/mindmap_architecture_thin.png" alt="MINDMAP architecture" width="300" style="display: block;"/>
    </p>
  </div>
  <div class="project-card__text">
    <h2 style="margin-top: 0;">Spatial Memory in Humanoid Manipulation</h2>
    <p>
    End-to-end learning has emerged as a promising approach towards intelligent robotic manipulators.
    Current approaches, however, lack spatial memory, which leads to surprising limitations in their capabilities.
    In this work we show how by providing a metric-semantic reconstruction to a denoising transformer based manipulation model,
    new capabilities for learning-based manipulation models are unlocked.
    </p>
    <p>
    Check out the <a href="https://arxiv.org/abs/2509.20297" title="MINDMAP paper">paper</a> and
    <a href="https://github.com/nvidia-isaac/nvblox_mindmap/" title="MINDMAP code">code</a>.
    </p>
  </div>
</div>
{% endcapture %}

<div class="notice--primary" style="float: left">
  {{ mindmap-text-2 | markdownify }}
</div>


{% capture perceptor-text %}
<div class="project-card">
  <div class="project-card__media">
    <p>
      <video width="300" autoplay loop muted playsinline style="display: block; margin-bottom: 10px;">
        <source src="/images/realsense_nvblox_humans.mp4" type="video/mp4">
      </video>
      <video width="300" autoplay loop muted playsinline style="display: block;">
        <source src="/images/warehouse_multicam_navigation.mp4" type="video/mp4">
      </video>
    </p>
  </div>
  <div class="project-card__text">
    <h2 style="margin-top: 0;">NVIDIA Perceptor</h2>
    <p>
    We integrated <code>nvblox</code> into a system for Autonomous Mobile Robot (AMR) navigation.
    The system combines multi-cam real-time reconstruction with deep-learned stereo and visual motion tracking
    from a set of cameras that surround the robot.
    <code>nvblox</code> was upgraded with features for motion segmentation to support navigation in environments with moving elements in the scene.
    Check out the <a href="https://www.youtube.com/watch?v=w1EU3JT32Do" title="perceptor video">video</a> and 
    <a href="https://nvidia-isaac-ros.github.io/reference_workflows/isaac_perceptor/index.html" title="perceptor code">code</a>.
    </p>
  </div>
</div>
{% endcapture %}

<div class="notice--primary" style="float: left">
  {{ perceptor-text | markdownify }}
</div>

{% capture nvblox-text %}
<a href="https://youtu.be/afNVwoX_zd0"><video autoplay loop muted playsinline aria-label="Nvblox" style="float: left; padding-right: 20px; width: 45%"><source src="/images/desk_radio_x2_600px.mp4" type="video/mp4"></video></a>
## nvblox: GPU-Accelerated Real-time Reconstruction for Robotics
{:style="margin-top:-10px"}
`nvblox` is a real-time reconstruction library for NVIDIA GPUs, including embedded devices. 
The library has been used in robot navigation, robotic manipulator control, mapping and robot learing research.
The library is open-source. [Try it out!](https://nvidia-isaac.github.io/nvblox)
{% endcapture %}

<div class="notice--primary" style="float: left">
  {{ nvblox-text | markdownify }}
</div>


## Selected Publications

A full list of publications may be found my [google scholar page](https://scholar.google.ch/citations?hl=en&user=opWkjhsAAAAJ "Google Scholar").


{% capture freetures-text %}
<a href="/nvblox"><video autoplay loop muted playsinline aria-label="nvblox" style="float: left; padding-right: 20px; width: 45%"><source src="/images/3dmatch.mp4" type="video/mp4"></video></a>
<!-- ## Freetures: Localization in Signed Distance Function Maps -->
<h2> <a style="text-decoration:none; color:#494e52;" href="/nvblox" title="nvblox Project Page">nvblox: GPU-Accelerated Incremental Signed Distance Field Mapping</a> </h2>
{:style="margin-top:-10px"}
Alexander Millane\*, Helen Oleynikova\*, Emilie Wirbel, Remo Steiner, Vikram Ramasamy, David Tingdahl, Roland Siegwart  
**International Conference on Robotics and Automation (ICRA), 2024.** 

\* contributed equally

{% endcapture %}

<div class="notice--primary" style="float: left">
  {{ freetures-text | markdownify }}
</div>


{% capture freetures-text %}
<a href="/freetures"><video autoplay loop muted playsinline aria-label="Freetures" style="float: left; padding-right: 20px; width: 45%"><source src="/images/freetures_fade.mp4" type="video/mp4"></video></a>
<!-- ## Freetures: Localization in Signed Distance Function Maps -->
<h2> <a style="text-decoration:none; color:#494e52;" href="/freetures" title="Freetures Project Page">Freetures: Localization in Signed Distance Function Maps</a> </h2>
{:style="margin-top:-10px"}
Alexander Millane, Helen Oleynikova, Christian Lanegger, Jeff Delmerico, Juan Nieto, Roland Siegwart, Marc Pollefeys, and César Cadena   
**IEEE Robotics and Automation Letters, 2020.** 

{% endcapture %}

<div class="notice--primary" style="float: left">
  {{ freetures-text | markdownify }}
</div>


{% capture freespace-features-text %}
<a href="/freespace"><video autoplay loop muted playsinline aria-label="Freespace" style="float: left; padding-right: 20px; width: 45%"><source src="/images/freespace_features_fade.mp4" type="video/mp4"></video></a>
<!-- ## Free‑Space Features: Global Localization in 2D Laser SLAM Using Distance Function Maps
{:style="margin-top:-10px"} -->
<h2> <a style="text-decoration:none; color:#494e52;" href="/freespace" title="Free‑Space Features Project Page">Free‑Space Features: Global Localization in 2D Laser SLAM Using Distance Function Maps</a> </h2>
{:style="margin-top:-10px"}
Alexander Millane, Helen Oleynikova, Juan Nieto, Roland Siegwart, and César Cadena   
**IEEE International Conference on Intelligent Robots and Systems (IROS), 2019** 

{% endcapture %}

<div class="notice--primary" style="float: left">
  {{ freespace-features-text | markdownify }}
</div>


{% capture voxgraph-text %}
<a href="/voxgraph"><video autoplay loop muted playsinline aria-label="Voxgraph" style="float: left; padding-right: 20px; width: 45%"><source src="/images/voxgraph_fast.mp4" type="video/mp4"></video></a>
<!-- ## Voxgraph: Globally Consistent, Volumetric Mapping using Signed Distance Function Submaps
{:style="margin-top:-10px;"}-->
<h2> <a style="text-decoration:none; color:#494e52;" href="/voxgraph" title="Voxgraph Project Page">Voxgraph: Globally Consistent, Volumetric Mapping using Signed Distance Function Submaps</a> </h2>
{:style="margin-top:-10px;"}

Victor Reijgwart\*, Alexander Millane\*, Helen Oleynikova, Roland Siegwart, César Cadena, Juan Nieto   
**IEEE Robotics and Automation Letters, 2019**

\* contributed equally

{% endcapture %}

<div class="notice--primary" style="float: left">
  {{ voxgraph-text | markdownify }}
</div>

{% capture cblox-text %}
<a href="/cblox"><video autoplay loop muted playsinline aria-label="cblox" style="float: left; padding-right: 20px; padding-bottom: 40px; width: 45%"><source src="/images/machine_hall_rotate_combined.mp4" type="video/mp4"></video></a>
<!-- ## C-blox: A Scalable and Consistent TSDF-based Dense Mapping Approach
{:style="margin-top:-10px"} -->
<h2> <a style="text-decoration:none; color:#494e52;" href="/cblox" title="C-blox Project Page">C-blox: A Scalable and Consistent TSDF-based Dense Mapping Approach</a> </h2>
{:style="margin-top:-10px;"}
Alexander Millane, Zachary Taylor, Helen Oleynikova, Juan Nieto, Roland Siegwart, César Cadena   
**IEEE International Conference on Intelligent Robots and Systems (IROS), 2018**

{% endcapture %}

<div class="notice--primary" style="float: left">
  {{ cblox-text | markdownify }}
</div>


## Projects

{% capture mbzirc-text %}
<a href="https://www.youtube.com/watch?v=QB1Cw2m6Yh8"><video autoplay loop muted playsinline aria-label="Tricopter" style="float: left; padding-right: 20px; width: 45%"><source src="/images/mbzirc_2020_voliro_t_crop.mp4" type="video/mp4"></video></a>
## Autonomous Fire-Fighting
{:style="margin-top:-10px"}
In this project we built a system for autonomously finding fires in multi-story buildings as part of our entry to the [MBZIRC 2020 international robotics competition](https://www.mbzirc.com/ "MBZIRC"). The mission is completed by a collaborating robotic team, consisting of a hexacopter and a tricopter. The approach exploits the mapping and precise control capabilities of each of the vehicles respectively. If you're interested, check out our [video](https://www.youtube.com/watch?v=QB1Cw2m6Yh8 "Autonomous Firefighting").
{% endcapture %}

<div class="notice--primary" style="float: left">
  {{ mbzirc-text | markdownify }}
</div>

{% capture thermal-mapping-text %}
<a href="https://www.youtube.com/watch?v=49WiPHkkhBw"><video autoplay loop muted playsinline aria-label="Thermal Mapping" style="float: left; padding-right: 20px; width: 45%"><source src="/images/thermal_mapping.mp4" type="video/mp4"></video></a>
## Thermal Mapping
{:style="margin-top:-10px"}
In this work we showed a UAV building dense 3D maps, localizing within these maps, and autonomously navigating through narrow spaces to find potential injured people using a thermal camera. We demonstrated this at a search and rescue training site in Switzerland. If you're interested, check out our [video](https://www.youtube.com/watch?v=49WiPHkkhBw "Thermal Mapping").
{% endcapture %}

<div class="notice--primary" style="float: left">
  {{ thermal-mapping-text | markdownify }}
</div>


<!-- 
This is the front page of a website that is powered by the [academicpages template](https://github.com/academicpages/academicpages.github.io) and hosted on GitHub pages. [GitHub pages](https://pages.github.com) is a free service in which websites are built and hosted from code and data stored in a GitHub repository, automatically updating when a new commit is made to the respository. This template was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) created by Michael Rose, and then extended to support the kinds of content that academics have: publications, talks, teaching, a portfolio, blog posts, and a dynamically-generated CV. You can fork [this repository](https://github.com/academicpages/academicpages.github.io) right now, modify the configuration and markdown files, add your own PDFs and other content, and have your own site for free, with no ads! An older version of this template powers my own personal website at [stuartgeiger.com](http://stuartgeiger.com), which uses [this Github repository](https://github.com/staeiou/staeiou.github.io).

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
 -->
