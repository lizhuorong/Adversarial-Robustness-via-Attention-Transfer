# Adversarial-Robustness-via-Attention-Transfer
This directory contains implementation of an enhanced adversarial training paper as well as models pre-trained on CIFAR-10 and CIFAR-100.
## Pre-requesites

- TensorFlow 1.4 and Python 3.5 

- numpy==1.16.0
## Datasets
Download the dataset which you're going to use and put put them in the corresponding folder.

- [Cifar-10](http://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz)

- [Cifar-100](http://www.cs.toronto.edu/~kriz/cifar-100-python.tar.gz)

## Overview of the Code
The code consists of Python scripts and the file config.json that contains various parameter settings.
### Example usage
-	python train.py: trains the network, storing checkpoints along the way.
- python eval.py: an infinite evaluation loop, processing each new checkpoint as it is created while logging summaries. It is intended to be run in parallel with the train.py script.

## Pre-trained models and Results
Following set of pre-trained checkpoints released with this code:
|Model|Dataset|Nominal Accuracy|Accuracy on<br>FGSM|Accuracy on<br>IFGSM_8_2_20|Accuracy on<br>PGD_8_2_7|Accuracy on<br>PGD_8_2_20|
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
|[wider-ResNet-Cifar10](https://pan.baidu.com/s/1BnyDedq3FWmnFqEfiRL3Tg)<br>(access code: 7jds)|Cifar-10|91.89%|76.74%|63.98%|70.15%|63.81%|

|Model|Dataset|Nominal Accuracy|Accuracy on<br>FGSM|Accuracy on<br>IFGSM_8_2_20|Accuracy on<br>PGD_8_2_10|Accuracy on<br>PGD_8_2_20|
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
|[wider-ResNet-Cifar100]( https://pan.baidu.com/s/1BnyDedq3FWmnFqEfiRL3Tg)<br>(access code: 7jds)|Cifar-100|76.22%|62.65%|28.84%|35.03%|28.72%|
				
## Acknowledgments
Code referred to the implementation of the [paper](https://arxiv.org/abs/1706.06083).
