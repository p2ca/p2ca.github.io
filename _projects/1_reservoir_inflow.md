---
layout: page
title: domain-adaptive reservoir inflow forecasting
description: what should transfer when hydroclimate shifts, and what should not
img: assets/img/reservoir_tsne.png
importance: 1
category: research
related_publications: true
---

Reservoirs with long, clean inflow records are the exception. Most sites we care about are data-scarce, so
the usual move is to train on data-rich reservoirs and transfer. The difficulty is that a snow-dominated
basin and a rain-dominated basin do not merely differ in scale — they are governed by different processes.
Aligning their representations wholesale forces genuinely site-specific structure to be shared, and accuracy
at the target site suffers.

The t-SNE above shows the problem directly: rain and snow reservoirs occupy visibly distinct regions of input
space, while the source/target split cuts across both. Whatever transfers has to survive that gap.

**DARSD-ResMetaLSTM** takes a different route from alignment. We organize reservoir information into three
sources — the dynamic hydrometeorological sequence, static reservoir attributes, and latent reservoir
context — then encode the sequence with reservoir-specific context and *decompose* the resulting latent state
into shared and reservoir-specific components using a learnable invariant basis. Static attributes are then
used to refine the decomposed forecast state, rather than being concatenated as raw features.

Evaluated on 33 U.S. reservoirs across six snow/rain transfer scenarios, the method outperforms alignment
baselines in **both** cross-regime directions — snow→rain and rain→snow — which alignment methods typically
fail to do symmetrically. The result supports the central claim: explicit decomposition makes reservoir
information usable under domain shift in a way that implicit alignment does not.

This work was carried out with collaborators at Oak Ridge National Laboratory and Stevens Institute of
Technology, and appears at the ACM AI Leadership Summit 2026 {% cite song2026darsd %}. An extended version is
in preparation.
