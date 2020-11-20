---
title: Chero
summary: Affordable, Quasi-Direct Drive Robot Manipulator
abstract: "Affordable, Quasi-Direct Drive Robot Manipulator."
date: "2019-11-27T00:00:00Z"
external_link: ""

image:
  caption: '[Chero: Prototype 1]()'
  focal_point: 'center'

#links:
#- icon: door-open
#  icon_pack: fas
#  name: website
#  url: https://summer-of-blogdown.netlify.com/
#- icon: github
#  icon_pack: fab
#  name: materials
#  url: https://github.com/rstudio-education/summer-of-blogdown-19
#- icon: flask
#  icon_pack: fas
#  name: demo site
#  url: https://kellykapowski.netlify.com/

categories:
- Hardware Projects
tags:
- hardware 
- wip

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

---
<DIV align="justify">

1. [What and why](#what-and-why)
2. [Previous works](#previous-works)
3. [What makes it special](#what-makes-it-special)
4. [Status](#status)
5. [Going Further](#going-further)


## What and Why

Chero is my acronym for  Chef-Robot, an ongoing project motivated by my desire to have a personal robot arm to experiment with. My long term dream of such a robot was triggered into action by the  MIT Collaborative Intelligence Challenge 2019, in which I gave a try. In addition, it as an interesting challenge and learning oppertunity to build such a system from grounds up - mechanical design-electronics controls.

## Previous Works

Direct drive robots are, as the name implies, are robots in which the motors directly drive the shaft without using a gearbox. It was introduced by Asada et al as early as early 80s [[1]](https://www.ri.cmu.edu/pub_files/pub4/asada_haruhiko_1981_1/asada_haruhiko_1981_1.pdf),[[2]](https://mitpress.mit.edu/books/direct-drive-robots). Direct drive robots have many inherent advantages like better torque control, dynamic response, zero backlash and friction etc. Despite all these advantages, the main disadvantage that prevented direct drive robots from becoming mainstream is mainly the low torque density of electrical motors. However, recent advancements in technology has brought us high torque BLDC motors, which are used either used directly or in combination with a  low gear ratio (<10) reducer. Notable robots include berkeley openarms[[3]](https://berkeleyopenarms.github.io/),   and numerous quadrupeds like MIT Cheetah [4](https://ieeexplore.ieee.org/document/6631038) and works by Gavin Kenneally et al[[5]](https://ieeexplore.ieee.org/document/7403902).

## What makes it special
1. Quasi-Direct Drive
2. Spherical shoulder and wrist joints
3. Redundant Robot - 7DOF
4. Cheap and affordable

The Quasi- Direct drive system consists of timing belt driven axes with a reduction ratio of 3. High torque density gimbal BLDC motors are used to actuate these joints.

The robot also has spherical joints at both the shoulder and the wrist, which matches closely with human arms.  It is shown that such a wrist design can be quite helpful in dexterous manipulation applications [[6]](https://ieeexplore.ieee.org/document/8624352)

## Status
The design is almost complete, parts machined-3dprinted and a video of first 4 DOF can be seen below
{{< youtube R1Q4KODC1f4 >}}

A 3DOF spherical wrist is also designed and assembled. It will be attached soon.



## Going Further
Implementing controllers, integrating with Drake

</DIV>



