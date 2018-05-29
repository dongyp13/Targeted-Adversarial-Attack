# Targeted-Adversarial-Attack

## Introduction
This repository contains the code for the top-1 submission to [NIPS 2017: Targeted Adversarial Attacks Competition](https://www.kaggle.com/c/nips-2017-targeted-adversarial-attack).

## Method
We use the momentum iterative method to generate adversarial examples. We summarize our algorithm in [Boosting Adversarial Attacks with Momentum](https://arxiv.org/pdf/1710.06081.pdf) (CVPR 2018, Spotlight).

We notice that targeted attacks have little transferability. The finding is drawn not only from our experiments but also from other submissions to this competition. We think that it's hard to find transferable adversarial examples for the ImageNet dataset with a large number of classes (i.e., 1000), because the decision boundary between two classes may not exhibit the same properties for different models.

### Citation
If you use momentum iterative method for attacks in your research, please consider citing

    @inproceedings{dong2018boosting,
      title={Boosting Adversarial Attacks with Momentum},
      author={Dong, Yinpeng and Liao, Fangzhou and Pang, Tianyu and Su, Hang and Zhu, Jun and Hu, Xiaolin and Li, Jianguo},
      booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
      year={2018}
    }

## Implementation

### Models
The models can be downloaded [here](http://ml.cs.tsinghua.edu.cn/~yinpeng/nips17/targeted/models.zip).

If you want to attack other models, you can replace the model definition part to your own models.

### Cleverhans
We also implement this method in [Cleverhans](https://github.com/tensorflow/cleverhans/blob/master/cleverhans/attacks.py#L454-L605).

## Non-targered Attacks
Please find the non-targeted attacks at [https://github.com/dongyp13/Non-Targeted-Adversarial-Attacks](https://github.com/dongyp13/Non-Targeted-Adversarial-Attacks).
