---
layout: default
title: "Large-Scale Cardiac Image Analytics"
date: 2025-12-03 12:00
speaker: "Jinming Duan (University of Manchester)"
has_link: true
---


## {{ page.speaker }}: {{ page.title }}

**{{ page.date | date: "%d-%m-%Y %H:%M" }}**
in **Law LT3 116**

## Abstract


## Speaker Bio
Dr. Jinming Duan received his PhD from the University of Nottingham, followed by postdoctoral research at Imperial College London. In 2019, he joined the University of Birmingham as a lecturer and was awarded Honorary Associate Professor in 2024. He is now an Associate Professor at the University of Manchester. Dr. Duan has published over 150 papers in leading journals such as The Lancet, Nature Machine Intelligence, TPAMI, TMI, and TIP, with a focus on machine learning and imaging methods in medical and cardiovascular applications. He has presented his work at major conferences like MICCAI, CVPR, ECCV, ICCV, NeurIPS, and AAAI. Dr. Duan was named a Turing Fellow by The Alan Turing Institute and serves on an Associate Editor for several scientific journals, including IEEE TNNLS and IEEE TCI. Dr. Duan has received multiple international competitions, including 2nd place in the 2023 MICCAI Learn2Reg Challenge, 2nd place in the 2023 ISBI RnR-ExM Challenge, 1st place in the 2022 MICCAI Learn2Reg Challenge, and 2nd place in the 2019 Facebook fastMRI International Challenge.


## Recording
This presentation will begin by detailing how domain knowledge can be effectively incorporated into neural network architectures for pairwise medical image registration. I will highlight how such integration improves the speed, accuracy, and data efficiency of the registration process, addressing the challenges posed by large and complex medical datasets.
I will then explore model-driven groupwise registration techniques for atlas construction. The resulting atlas enables one-shot segmentation, where a single manual annotation of the template image can be accurately propagated to individual subjects through the learned deformations. Building on the estimated atlas geometry and deformations, I will further introduce a novel statistical shape modelling strategy that implicitly generates new anatomical heart shapes. This method maintains exact point-to-point correspondence and prevents mesh folding, while ensuring anatomical plausibility using diffeomorphic transformations.
