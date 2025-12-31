---
title: "Accessible, At-Home PD Detection via Multi-Task Video Analysis (UFNet)"
collection: projects
category: published
permalink: /projects/ufnet-multitask-video-pd-screening
layout: single
author_profile: true
year: 2025
order: 2
publication: "AAAI-25"
paperurl: "https://arxiv.org/abs/2406.14856"
---

We developed **UFNet**, an uncertainty-calibrated multimodal fusion network that detects Parkinson’s disease from at-home webcam tasks (finger tapping, smiling, and speech), using only a computer with a camera, microphone, and internet connection. The work introduces the first large-scale, multi-task PD video dataset and shows that fusing task-specific models with uncertainty-aware attention improves both performance and safety for remote screening. <!--more-->
- Collected a **multi-task video dataset** of 845 participants (272 with PD) performing three standardized tasks (finger-tapping, smile, and pangram speech), yielding 1,102 complete multi-task sessions and 3,306 total videos for model development and evaluation.
- Built **task-specific shallow neural networks** with Monte Carlo (MC) dropout for each modality, extracting clinically motivated features (finger-tapping kinematics, facial action/motion features, and WavLM speech embeddings) and estimating prediction uncertainty.
- Proposed **UFNet**, which projects task-specific features into a shared space and uses *uncertainty-calibrated self-attention* to down-weight noisier or less reliable tasks while leveraging complementary information across modalities.
- Demonstrated that UFNet **outperforms single-task models and standard multimodal fusion baselines**, achieving around 87–88% accuracy and ~93% AUROC on a subject-separated test set, with further gains when withholding low-confidence predictions.
- Incorporated **confidence-aware decision policies** (MC dropout, conformal prediction, and calibration techniques) to selectively abstain on uncertain cases, improving calibration and reducing harmful mispredictions in a screening context.
- Showed **no significant performance bias across sex and race**, and best performance for individuals aged 50–80, while also validating the approach on the external YouTubePD dataset to test robustness across different video sources.
