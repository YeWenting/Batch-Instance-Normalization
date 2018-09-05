# Batch-Instance-Normalization

This repository provides an example of using [Batch-Instance Normalization](https://arxiv.org/abs/1805.07925) for classification on CIFAR-10/100, written by [Hyeonseob Nam](https://www.linkedin.com/in/hyeonseob-nam/) and [Hyo-Eun Kim](https://www.linkedin.com/in/hekim0530/) at [Lunit, inc.](https://lunit.io/)

Acknowledgement: This code is based on [Wei Yang's pytorch-classification](https://github.com/bearpaw/pytorch-classification)

## Citation
If you use this code for your research, please cite:

Hyeonseob Nam and Hyo-Eun Kim, *Batch-Instance Normalization for Adaptively Style-Invariant Neural Networks*, arXiv preprint, 2018.
(To appear in NIPS 2018)
[[paper]](https://arxiv.org/abs/1805.07925)

## Prerequisites
- [PyTorch 0.4.0](https://pytorch.org/)
- Python >= 3.5
- Cuda >= 8.0

## Training Examples
Training ResNet-50 on CIFAR-100 using **Batch Normalization**
```
python main.py --dataset cifar100 --depth 50 --norm bn --checkpoint checkpoints/cifar100-resnet50-bn
```
Training ResNet-50 on CIFAR-100 using **Instance Normalization**
```
python main.py --dataset cifar100 --depth 50 --norm in --checkpoint checkpoints/cifar100-resnet50-in
```
Training ResNet-50 on CIFAR-100 using **Batch-Instance Normalization**
```
python main.py --dataset cifar100 --depth 50 --norm bin --checkpoint checkpoints/cifar100-resnet50-bin
```

## LICENSE
This repository is released under **the MIT License**
