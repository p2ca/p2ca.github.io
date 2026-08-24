---
layout: page
title: UAV 3D reconstruction and target detection
description: point cloud reconstruction from an airborne RealSense camera
importance: 4
category: coursework
---

Final project for Interdisciplinary Research and Practice: Intelligent Machine Vision at Tsinghua. Using an
Intel RealSense depth camera mounted on a UAV, I reconstructed the surrounding environment as a 3D point
cloud and performed target detection directly on the reconstructed geometry.

Most of the real work was in the stitching. Point clouds captured from a moving airborne platform arrive with
noisy pose estimates, so I used Open3D to debug and tune the camera integration, the stitching procedure, and
the registration algorithms until consecutive frames aligned reliably enough for detection to be meaningful.
