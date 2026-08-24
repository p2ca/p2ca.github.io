---
layout: page
title: camouflaged and salient object detection
description: separating objects that are visually entangled with their background
importance: 2
category: research
---

At Tsinghua's Institute of Information Processing, I worked on improving detection accuracy for objects that
are hard to segment because they *resemble* their surroundings — the camouflaged object detection (COD)
setting — and on how it relates to salient object detection (SOD), where the object is instead the most
conspicuous thing in the frame.

The two tasks are usually treated separately, but they are close to inverses of each other, and the
intermediate representations produced during encoding and decoding carry information useful to both. I built
a VGG-based training pipeline in Python that combined COD and SOD supervision together with images generated
at the encoder–decoder stages, expanded the training set, and iterated on the network architecture and loss
functions to raise recognition accuracy.

The motivating application was obstacle avoidance for autonomous driving, where the failure case that matters
is exactly the one COD studies: an obstacle that blends into the road scene and is therefore detected late.

Looking back, this is the same question I now work on in time series — which part of a representation is
genuinely about the object, and which part is about the background it happens to sit in.
