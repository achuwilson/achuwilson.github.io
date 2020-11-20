---
title: 2048 Solver Robot
summary: Solving a 2048 game using AI, computer vision and a real robot
abstract: "Solving a 2048 game using AI, computer vision and a real robot."
date: "2015-10-27T00:00:00Z"
external_link: ""

image:
  caption: '[Chippu: Prototype 1]()'
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
2. [How](#How)
3. [Result](#result)


## What and Why

2048[[1]](https://en.wikipedia.org/wiki/2048_(video_game))  is a single-player sliding block puzzle game. The objective of the game is to slide numbered tiles on a grid to combine them to create a tile with the number 2048.

This was a weekend hobby project, to make use of a robot arm, computer vision and AI techniques to solve and play the game. 

## How

The state of the game is inferred from the smartphone screen. Screenshots are perodically captured via the ADB interface. The image is pre-processed and an OCR is done to detect the digits on each tile. 

Given the current game state, an alpha-beta pruning algorithm predicts the next best action. The action space is swipe in Left/Right/Up/Bottom directions. The robot arm then would move towards the screen and make the swipe

## Result

See for yourself!.

{{< youtube hUNTeZJSUWE >}}

It not only wins the game, but also scores unbelievable scores.

</DIV>



