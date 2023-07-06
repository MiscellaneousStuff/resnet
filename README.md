# ResNet

## About

Re-implementation of ResNet.
[Original paper](https://arxiv.org/pdf/1512.03385.pdf).

## Method

### Paper Details

- Image scaled to 224x224 crop (same as AlexNet).
  Per-pixel mean subtracted.
- Batch norm after conv and before activation.
- Initiaise weights based on He initialisation.
- SGD Initialisation with Batch Size := 256.
- Start LR := 0.1, /= 10 on plateau. 6,000,000 iters.
- Weight decay := 0.0001. Momentum of 0.9.
- No dropout.
- 10 crop testing?

## TODO

- [x] ResNet
   - [x] Model
   - [x] Train Code
- [x] MNIST (~98%)
- [x] CIFAR-10 (83.94%)
- [ ] Tiny ImageNet