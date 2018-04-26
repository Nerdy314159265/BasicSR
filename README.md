# BasicSR

BasicSR mainly contains 3 parts:

1. general SR models
1. [SRGAN model](https://arxiv.org/abs/1609.04802)
1. [SFTGAN model](http://mmlab.ie.cuhk.edu.hk/projects/SFTGAN/)

Now it supports 1 and 2.

The repo is still under development. There may be some bugs :-)

<!-- ### Table of Contents
1. [Introduction](#introduction)
1. [Introduction](#introduction)

### Introduction -->

### Prerequisites

- Linux
- Python3
- Pytorch 0.3.1
- NVIDIA GPU + CUDA CuDNN

### Codes descriptions

Please see Wiki pages(https://github.com/xinntao/BasicSR/wiki), which contains:
- [[data] instructions](https://github.com/xinntao/BasicSR/wiki/%5Bdata%5D-instructions)
- [[options] instructions](https://github.com/xinntao/BasicSR/wiki/%5Boptions%5D-instructions) (including all configuration descriptions)


### Getting Started
- How to train a model
1. prepare your data (it's better to test whether the data is ok using `test_dataloader`)
1. modify the corresponding training json file in `options/train/xxx.json`
1. train the model with the command `python3 train.py -opt options/train/SRResNet.json`

- How to test a model
1. prepare your data and pretrained model
1. modify the corresponding testing json file in `options/test/test.json`
1. test the model with the command `python3 test_LRinput.py -opt options/test/test.json`





