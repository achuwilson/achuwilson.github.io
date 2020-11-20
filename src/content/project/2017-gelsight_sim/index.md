---
title: Gelsight Simulation 1
summary: Simulating Gelsight Sensor by generating pointcloud
abstract: "Simulating Gelsight Sensors using Raytracing"
date: "2017-11-27T00:00:00Z"
external_link: ""

image:
  caption: '[Gelsight Sim]()'
  focal_point: 'center'
  preview_only: true

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
- Software Projects
tags:
- software 


url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

---
<DIV align="justify">

1. [What and why](#what-and-why)
2. [How](#how)
3. [Result](#result)


## What and Why

This is my initial approach in modelling the behaviour of GelSight tactile sensors in simulation. I resorted to simulation as I did not have access to the real sensor or resources to build one. 

## How
I used the physics simulator Bullet. It had softbody simulation, which I thought would be useful for simulating the elastomer of GelSight. But it turned out that the softbody simulation was a basic and needed much more development. So, I indirectly modelled Gelsight using the raytest functionality in bullet. It returns the depth at which a ray makes contact with a solid body.

## Result

Following is the video of the simulated gelsight gripper. The Kuka iiwa has a WSG 50 gripper fitted with a gelsight sensor. The sensor has a sensing area of 24x24mm and has a resolution of 256x256 pixels in the planar sensing area. It outputs standard ROS 3D pointcloud data, which is displayed in RViz.The simulation was run in my laptop and the pointcloud could be generated at 5Hz 
{{< youtube IO02smLcDQE >}}

Even though I could simulate the sensor, I soon ran into comptational limits of my laptop. </DIV>



