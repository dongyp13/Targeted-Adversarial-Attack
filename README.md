# Targeted-Adversarial-Attack

## Introduction
We propose a targeted momentum iterative fast gradient sign method. This method won the first place in [NIPS 2017: Targeted Adversarial Attacks Competition](https://www.kaggle.com/c/nips-2017-targeted-adversarial-attack/leaderboard).

## Method
We noticed that targeted attacks have little transferability. So we instead only focus on white-box targeted attack. We also use the iterative fast gradient sign approach with momentum, which is summarized in [Boosting Adversarial Attacks with Momentum](https://arxiv.org/pdf/1710.06081.pdf). We ensemble five models in our code.

## Models
The models can be downloaded [here](http://ml.cs.tsinghua.edu.cn/~yinpeng/nips17/targeted/models.zip).

## Non-targered Attacks
Please find the non-targeted attacks at [https://github.com/dongyp13/Non-Targeted-Adversarial-Attacks](https://github.com/dongyp13/Non-Targeted-Adversarial-Attacks).
