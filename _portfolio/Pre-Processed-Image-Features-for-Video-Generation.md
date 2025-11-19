---
title: "Pre-Processed Image Features for Video Generation"
use_math: true
excerpt: "
![status: ongoing](https://img.shields.io/badge/status-ongoing-blue.svg)
![target: 02/2026](https://img.shields.io/badge/target-04/2026-yellow.svg)<br/>
A pre-processing technique to improve the training and inference times of video generation models.
"
collection: portfolio
---

![status: ongoing](https://img.shields.io/badge/status-ongoing-blue.svg)
![target: 02/2026](https://img.shields.io/badge/target-04/2026-yellow.svg)

Video generation mostly involves generating a series of images such that an image at time $$t_1$$ closely resembles the images at time $$t_0$$ and $$t_2$$, but with minor variations to account for the motion of objects within the scene. This project aims to develop a pre-processing technique to improve the training time of video generation models by having the models use and generate smaller dimensional data that is devoid of most of the still parts of the images that have to be continuously generated at each time step.
