# MNIST-SVHN_AdaIN
This project is based on [Arbitrary Style Transfer in Real-time with Adaptive Instance Normalization](https://arxiv.org/pdf/1703.06868.pdf) by Xun Huang and Serge Belongie from the Department of Computer Science & Cornell Tech, Cornell University. 
### Adaptive Instance Normalization
Adaptive Instance Normalization is a normalization method that aligns the **mean** and **variance** of the content features with those of the style features. Unlike Batch Normalization, Instance Normalization or Conditional Instance Normalization, **AdaIN has no learnable affine parameters**. Instead, it adaptively computes the affine parameters from the style input:
![AdaIN](https://www.henryailabs.com/ArticlePictures/StyleGAN-3.jpg)
### Style Transfer Network
The AdaIN style transfer network takes a **content image** and an arbitrary **style image** as inputs, and synthesizes an output image that recombines the content and style of the respective input images. The network adopts a simple encoder-decoder architecture. The **VGG**, in this project, was replaced by a much smaller **CNN AE**.
![Style Transfer Network](https://www.researchgate.net/publication/333617596/figure/fig1/AS:766279258480641@1559706620845/AdaIN-style-transfer-architecture-4.ppm)
