---
layout: post
title:  "Our Advanced Weed Detection Model"
date:   2024-11-06 10:00:00 +0100
categories: blog
---
Weeds significantly impact agricultural production, and traditional weed control methods often harm soil health and the environment. This study aims to develop deep learning-based segmentation models in identifying weeds in potato fields captured by Unmanned Aerial Vehicle (UAV) orthophotos and to explore the effects of weeds on potato yield. UAVs were used to collect RGB data from potato fields, flying at an altitude of 10m, with Real-ESRGAN Super-Resolution (SR) enhancing image resolution. We applied the Segment Anything Model (SAM) to do semi-automatic annotation, followed by training the YOLOv8 and MASK-RCNN models for segmentation. Also we used ANOVA and linear regression to analyze the effects of weeds and nitrogen fertilizer on yield. Results showed that the detection accuracy mAP50 scores for YOLOv8 and Mask R-CNN were 0.902 and 0.920, respectively, with the Real-ESRGAN-enhanced model achieving 0.909. When multiple weed types were present, accuracy decreased to 0.86.

![model inference]({{ site.baseurl }}/assets/images/maskrcnn_example.jpg)

[Paper](https://www.biorxiv.org/content/10.1101/2024.08.13.607729v1.full)