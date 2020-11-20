---
title: BlindGrasp
summary: Grasping in vision denied environments using Tactile Sensing.
abstract: "Grasping in vision denied environments using Tactile Sensing"
date: "2020-07-27T00:00:00Z"
external_link: ""

image:
  caption: '[BlindGrasp Image]()'
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
- wip  


url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

---
<DIV align="justify">

1. [What and why](#what-and-why)
2. [Previous works](#previous-works)
3. [How](#how)
4. [Status](#status)



## What and Why

BlindGrasp, as the name implies, aims at grasping objects when the robot's eyes are blindfolded. This idea had been lingering in my mind, ever since I came across the GelSight optical tactile sensor. It is a tough and challenging problem and I have been making slow, yet good progress. This is the main project that I am spending my time now and has helped us to be the finalist in the *Kuka Innovation Award 2021*


Humans have excellent grasping capabilities in unstructured environments which are still unmatched by robots. This can be attributed to the dexterous human hand, robust visual and tactile sensing capabilities as well as to the intelligent brain which makes conscious and subconscious decisions. 


Visual sensing is traditionally used extensively in robotics when compared to tactile sensing. Tactile sensing is harder, mainly due to the difficulty in interpreting and making sense of the complex tactile signals. The recent developments in machine learning - particularly Deep Reinforcement Learning has opened new possibilities in the making usage of such complex data.


We humans can effortlessly put a hand inside a bag, search by moving it around and pick up an item or we can use our hands to dig or sieve through granular medium like sand and pick up an object. This project explores building a system which learns manipulation and grasping skills in such vision denied environments.


## Previous Works


Grasping objects, using tactile sensing alone as well as in granular media are explored more recently. Following are some of the early works.


1. [Reactive Grasping Using Optical Proximity Sensors](http://www.robotics.stanford.edu/~ang/papers/icra09-ProximityGrasping.pdf) by Kaijen Hsaio et al.
2. [A Deep Learning Approach to Grasping the Invisible](http://choice.umn.edu/deep-learning-approach-grasping-invisible), by Yang Yang et al.
3. [Vibro-Tactile Foreign Body Detection in Granular Objects based on Squeeze-Induced Mechanical Vibrations](https://ieeexplore.ieee.org/abstract/document/9158928) by Togzhan Syrymova et al.
4. [MAT: Multi-Fingered Adaptive Tactile Grasping via Deep Reinforcement Learning](http://arxiv.org/abs/1909.04787) by Bohan Wu et al.
5. [Learning to Grasp without Seeing](http://arxiv.org/abs/1805.04201) by Adithyavairavan Murali et al.
6. [Multimodal Haptic Perception within Granular Media via Recurrent Neural Networks](#) by S.Jia et al.
 
There are almost no works combining tactile sensing- exploration and grasping objects in granular media

## How

Bringing such novel manipulation capabilities to robots calls for better robot hands as well as algorithms. The stated goals of the project are

1. Building a novel tactile sensing capable gripper
2. Develop AI techniques to make the robot learn how to explore, detect and grasp objects in unstructured-vision denied environments where tactile sensing only could be used.

The Tactile Sensing Gripper consists of a two finger parallel jaw gripper, with tactile sensing capabilities. Similar to the human fingers, the inner surface of the fingers would be having a high spatial resolution tactile sensing capability and the outer surface comparatively lower resolution. The highly sensitive inner surface of the finger helps in recognizing objects from their shape, texture as well as in fine manipulation skills. The lower sensitive outer surface helps in detecting the presence of nearby objects via contact.



The AI System consists of a Deep Reinforcement Learning Agent that learns how to explore the environment and to recognize/differentiate objects and pick them up. The agent uses data from the two types of tactile sensors on each of the fingers, proprioception and force sensor data from the robot arm. The agent decides the direction of motion of the end effector and the control of the gripper.

As a relatively simple task to start with, grasping specific objects from an environment similar to the following setup will have to be acheived using the tactile sensing alone.

{{< imgresize pick1.png "450x450" "picking task 1" >}}
 

Ultimately, the robot is expected to learn how to pick up objects under the granular media as in the following simulation. 

{{<youtube a2rk8dN3KsA >}}

## Status

A novel gripper, with tactile sensing around the finger is built and we are collecting data from the real world environment. This would be augmented with data from the simulated environment and human demonstrations to train the RL agent for the task. 

More updates coming soon, as it is an ongoing project..!

</DIV>



