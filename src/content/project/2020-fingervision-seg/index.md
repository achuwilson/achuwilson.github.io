---
title: Background segmentation
summary: Background Segmentation for Fingervision Tactile Sensor
abstract: "Background Segmentation for Fingervision Tactile Sensor"
date: "2020-01-27T00:00:00Z"
external_link: ""

image:
  caption: '[Segmented Image]()'
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
2. [Previous works](#previous-works)
3. [How](#how)
4. [Result](#result)


## What and Why

FingerVision is an optical tactile sensor[[1]](https://ieeexplore.ieee.org/document/7803400), which provides the RGB image of the object within the fingers in addition to the contact forces from the optical markers.

Since the sensor captures the image of the background also in addition to the object, we need to seperate out the object and the background.

## Previous Works

*to update later*

## How
A deep learning approach is used to segment the objects and the background. Training data is collected, manually labelled and a U-Net based network is trained.
The training acheives good accuracy in a couple of tens of minutes. Transfer learning methods could be used to quickly adapt to new environments.

## Result

It works, as expected.

{{< youtube XZOl3pS5oLY >}}

The left side shows the raw sensor image and the right one is the segmented image output. 

</DIV>



