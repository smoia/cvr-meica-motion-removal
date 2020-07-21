---
layout: post
title: Background
description: In tasks where noise highly correlates with the signal of interest, denoising is difficult due to the tradeoff between effective denoising and signal conservation. This is the case of Breath-Hold (BH) induced Cerebrovascular Reactivity (CVR).
image: background.png
---

Functional MRI presents different sources of noise: hardware related artifacts, inflow effects, motion-related signal changes, cardiac and respiratory related fluctuations. Removal of task-correlated noise, such as in a Breath-Holding (BH) paradigms, is particularly challenging, due to the tradeoff between effective denoising and signal conservation [1]. Common denoising of fMRI data is done via nuisance regression of realignment parameters, their temporal derivatives and slow frequency drifts. Alternatively, independent component analysis (ICA) can also be employed to decompose the signal into different sources, identifying those related to noise, and use this information during nuisance regression [2]. In particular, multi-echo ICA (ME-ICA) enables to effectively identify non-BOLD (e.g. movement) artifacts [3-4] from BOLD-related components, which can enhance the contrast to noise ratio of the signal in addition to optimal combination of the echoes.
This work evaluates different denoising variants to clean ME-fMRI data acquired during a BH task where noise highly correlates with the cerebrovascular reactivity response (CVR) of interest (e.g. movement linked to deep breaths).
