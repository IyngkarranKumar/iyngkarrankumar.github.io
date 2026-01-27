---
title: Emergent Abilities in Language Reasoning Models at Inference Time
layout: home
excerpt: Investigating the predictability of test-time scaling in language models
order: 1
---

Sharp, non-linear jumps in model performance have previously been observed when language model size and training compute are scaled [(Wei et al., 2022)](https://arxiv.org/abs/2206.07682), [(Berti et al., 2025)](https://arxiv.org/abs/2503.05788). This poses a challenge to forecasting model capabilities; ideally, all capabilities of interest would display smooth, continuous scaling. 
Additionally, recent trends have seen a shift away from training compute scaling towards inference (or test-time) compute scaling, with test-time compute scaling laws being proposed [(Wu et al., 2025)](https://arxiv.org/abs/2408.00724), [(Snell et al., 2024)](https://arxiv.org/abs/2408.03314). However, this work has not explored the extent to which this scaling is smooth and continuous, or sharp and non-linear (emergent). This project investigates the presence of emergent scaling in language reasoning models at test-time.

[See the paper here](/assets/docs/Emergent_Abilities_in_Large_Language_Models_at_Inference_Time__ICML_2701.pdf)

[Codebase](https://github.com/IyngkarranKumar/test_time_emergent_scaling/tree/clean_public_branch)