---
layout: default
modal-id: 2
date: 2019-06-16
img: monoresmatch.gif
alt: image-alt
project-date: June 2019
conference: IEEE CONFERENCE ON COMPUTER VISION AND PATTERN RECOGNITION (CVPR)
keywords: [Monocular Depth Estimation, Deep Learning] 
title: Learning monocular depth estimation infusing traditional stereo knowledge

---

## LEARNING MONOCULAR DEPTH ESTIMATION INFUSING TRADITIONAL STEREO KNOWLEDGE

Depth estimation from a single image represents a fascinating, yet challenging problem with countless applications. Recent works proved that this task could be learned without direct supervision from ground truth labels leveraging image synthesis on sequences or stereo pairs. Focusing on this second case, in this paper we leverage stereo matching in order to improve monocular depth estimation. To this aim we propose monoResMatch, a novel deep architecture designed to infer depth from a single input image by synthesizing features from a different point of view, horizontally aligned with the input image, performing stereo matching between the two cues. In contrast to previous works sharing this rationale, our network is the first trained end-to-end from scratch. Moreover, we show how obtaining proxy ground truth annotation through traditional stereo algorithms, such as Semi-Global Matching, enables more accurate monocular depth estimation still countering the need for expensive depth labels by keeping a self-supervised approach. Exhaustive experimental results prove how the synergy between i) the proposed monoResMatch architecture and ii) proxy-supervision attains state-of-theart for self-supervised monocular depth estimation

## Architecture