---
title: "Automatic Refueling Robot"
draft: false
date: 2020-10-25
description: "This project is the starting point of my scientific research. Through my own exploration, I learned several programming languages, Linux usage, basic computer vision algorithms, Socket communication and GUI programming. I got started with machine learning and deep learning. Meanwhile, I accumulated some experience in edge device transplantation."
tags:
  - Projects
---
This project is the starting point of my scientific research. Through my own exploration, I learned several programming languages, Linux usage, basic computer vision algorithms, Socket communication and GUI programming. I got started with machine learning and deep learning. Meanwhile, I accumulated some experience in edge device transplantation.

### Condition Guided Detection
In the early stage, I was exposed to C++ and Python while trying traditional CV algorithms.
I used canny operator, support vector machine (SVM), cascade classifier and other technologies to implement the first demo using a large number of artificial rules.

![Enhanced Detection](enhance_detect.mp4)

### Deep Learning & Edge Computing
Gradually, I began to try to get in touch with deep learning. Tensorflow and darknet were the deep learning frameworks I initially used. Although PyTorch is used extensively in my later scientific research, during the process I repeated routine operations such as environment configuration hundreds of times which lays the foundation for the future.
Meanwhile, I started to notice efficiency issues. I compared the fastest neural networks at the time and tried to find ways to deploy them on edge devices, such as Raspberry Pi + Intel Movidius (OpenVINO) or Nvidia Jetson Nano (CUDA).
Consequently, I also tried to build a thin client model based on Socket communication, using one host to process data from multiple edge devices.
All these contents were later integrated into a GUI program based on the C# .Net framework.

![Fast Detection](fast_detect.mp4)

### Stereo Camera & Radar
Even though our task was limited to visuals, I became interested in the entire pipeline.
I started thinking about how to use vision to guide the robotic arm to complete the refueling.
In order to obtain depth information, I learned stereo matching and introduced radar information to combat lighting problems.

![Depth Fetching](depth.mp4)

### 3D Printing & Robot Control
Finally, I modified a robotic arm model through 3D printing to achieve the functions required by the refueling robot.

![Robot Control](robot.mp4)