---
title: Self parking car
summary: A simple self parking car usinf IR distance sensors.
abstract: "A simple self parking car usinf IR distance sensors "
date: "2009-03-27T00:00:00Z"
external_link: ""

image:
  caption: '[Self Parking ]()'
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
- Hardware Projects
tags:
- embedded
- hardware


url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

---
<DIV align="justify">



 

1. [What and why](#what-and-why)
2. [How](#how)
3. [Result](#results)



## What and Why

This is a small side project during my undergraduate days, to master embedded systems and robotics skills. 

## How
The robot car consists of IR distance sensors on its sides and wheel encoders. These data streams are fed into a state machine, which looks for empty parking spots. If found any, the state machine would initialize the parking subroutine, and executes a parking maneuver.

{{< imgresize parkingcar.jpg "450x450" "parking robot car" >}}
The above image shows the setup used.

## Result


Some trials!
{{< youtube GDYHJPsIQ2M >}}


</DIV>



