---
title: "Paper Review 4 - SRResnet, SRGAN [Super Resolution]"
categories:
  - study
tags:
  - deep learning
  - Super Resolution
last_modified_at: 2019-07-22T23:11:00+09:00
comments: true
mathjax: true
sitemap :
  changefreq : daily
  priority : 1.0
---

# [Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial Network](https://arxiv.org/pdf/1609.04802.pdf)

- Accepted Conference Name & Year : CVPR 2017
- 1st Author Name & Institute : Christian Ledig, Twitter

## Contribution

- Resnet 구조를 SR 에 그대로 적용한 SRResnet은 안정적으로 깊은 모델을 학습할 수 있었다.
- 하지만 MSE loss 로 학습을 진행할 경우 image 가 smooth 하게 되기 때문에 texture 가 선명해지기 힘들다.
- 이런 문제를 해결하기 위해 GAN을 기반으로 하는 SRGAN은 Real patch 들의 분포를 학습해서 패턴을 만들기 때문에 굉장히 Realistic 하게 보이게 된다. 물론 GAN 특성 상 Ground truth 와는 다른 패턴이 되기도 한다.

## Proposed Architecture
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-09-22-Paper-Review-4-SRResnet-SRGAN-Super-Resolution/Untitled-e3d739d2-e7f7-4e6d-93a2-f33baf8f4622.png" alt="">
</figure> 
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-09-22-Paper-Review-4-SRResnet-SRGAN-Super-Resolution/Untitled-13c852de-b751-44a3-9edb-72a31c097a54.png" alt="">
</figure> 

## Dataset
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-09-22-Paper-Review-4-SRResnet-SRGAN-Super-Resolution/Untitled-87dee319-30b5-4fa9-935c-605f5d54b540.png" alt="">
</figure> 
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-09-22-Paper-Review-4-SRResnet-SRGAN-Super-Resolution/Untitled-00d7f15d-7a43-43d8-9dbd-12efc0586a88.png" alt="">
</figure> 

## Valuable Relative Works

- [Resnet](https://arxiv.org/pdf/1512.03385)
- [ESPCN](https://arxiv.org/pdf/1609.05158.pdf)
