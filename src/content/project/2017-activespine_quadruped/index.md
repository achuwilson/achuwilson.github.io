---
title: Quadruped with Active spine
summary: Mid air inertial re-orientation using an active spine
abstract: "Mid air inertial re-orientation using an active spine."
date: "2017-05-27T00:00:00Z"
external_link: ""

image:
  caption: '[Quadruped Active Spine]()'
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
2. [Previous Works](#previous-works)
3. [Results](#results)
4. [Status](#status)
5. [References](#references)


## What and Why

This is a side project to explore whether quadrupeds can be made to land on all four legs safely after they are dropped/thrown in random orientations.

## Previous Works

[Cat righting reflex](https://en.wikipedia.org/wiki/Cat_righting_reflex) been extensively studied before. In 1942 US Air Force played with kittens in microgravity. The same lab, in 1962, published a report titled [Weightless Man: Self-Rotation Techniques](http://www.dtic.mil/dtic/tr/fulltext/u2/400354.pdf), as a guidline for future astronauts on how to move around in zero gravity. 1960s. The falling cat was also studiedextensively by NASA to prepare the astronauts for Zero-G environments. A 1969 paper titled [A Dynamical Explanation of the Falling Cat Phenomenon](http://www.sciencedirect.com/science/article/pii/0020768369900869) explains this.

Past research attributes the cat reflex to law of conservation of momentem. Flexible bodies can generate internal forces and moments, by the motion of limbs. But the rest of the body rotates in opposite direction owing to the conservation of momentum, so that net angular momentum remains zero. However the rate of rotation can be controlled by extending or pulling back the limbs. Wikipedia summarises it to three key steps:


1.Bend in the middle so that the front half of their body rotates about a different axis from the rear half.
2.Tuck their front legs in to reduce the moment of inertia of the front half of their body and extend their rear legs to increase the moment of inertia of the rear half of their body so that they can rotate their front further (as much as 90°) while the rear half rotates in the opposite direction less (as little as 10°).
3.Extend their front legs and tuck their rear legs so that they can rotate their rear half further while their front half rotates in the opposite direction less.

Depending on the cat’s flexibility and initial angular momentum, if any, the cat may need to perform steps two and three repeatedly in order to complete a full 180° rotation.

Past works on using active spine in legged robots specialized rotation in the axis perpendicular to the saggital plane and was aimed at improving the gait. My research focusess on rotation in the axis perpendicular to the transverse plane. I developed an inertial reoreintation controller. It controls the extension and tucking in of the quadruped limbs, so that the cranial and caudal part rotates with different velocities owing to the conserved momentum. The controller thus uses the inertia of the quadruped to reorient itself.


## Results

A quadruped was modelled in the Bullet simulator and a simple state machine based controller was implemented. It works beautifully as in the following video

{{<youtube 4Hg29l2iCJo >}}

## Status

As the system is verified in simulation, now it has to be implemented in hardware. 
I am working on a small quadruped during freetime and it will be updated later.

Here are some photos of it in progress.

{{< imgresize quad1.jpg "450x450" "quadruped image 1" >}}
{{< imgresize quad2.jpg "450x450" "quadruped image 2" >}}


## References

will be updated later as time permits.

</DIV>



