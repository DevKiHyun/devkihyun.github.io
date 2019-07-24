---
title: "Paper Review 2 - VDSR [Super Resolution]"
categories:
  - study
tags:
  - deep learning
  - Super Resolution
last_modified_at: 2019-07-22T22:47:00+09:00
mathjax: true
sitemap :
  changefreq : daily
  priority : 1.0
---


# [Accurate Image Super-Resolution Using Very Deep Convolutional Networks](https://arxiv.org/pdf/1511.04587v2.pdf)

- Accepted Conference Name & Year : CVPR 2016
- 1st Author Name & Institute : Jiwon Kim, Seoul National University

## Contribution

- Resnet의 기법 중 skip-connection 을 이용해 아주 깊게 layer 를 쌓을 수 있게 되어됨.
- Resolution에서 선명함이라는 것은 Detail 한 부분이 결정 짓기 때문에 skip-connection 으로 input 을 output 에 넘겨주면 이 둘 간의 차이(Detail)에 좀 더 집중할 수 있다.
- 깊어진 네트워크에 따라 확장된 receptive field 덕에 더 많은 주변 픽셀 정보를 이용 할 수 있게 됨.
- 다양한 scale(2x,3x,4x)에 대한 이미지들을 동시에 학습시킨 multi-scale 모델을 구성해 더욱 적은 모델 용량으로도 좋은 성능을 보여줌.
- 더 깊은 모델의 가능성을 열게 됨.

## Proposed Architecture

<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-09-22-Paper-Review-2-VDSR-Super-Resolution/Untitled-b567e118-f2ae-4859-9f12-5926cdeb84cb.png" alt="">
</figure> 

## Dataset
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-09-22-Paper-Review-2-VDSR-Super-Resolution/Untitled-bd8eb022-47fe-41ae-8597-7396aee7dcc0.png" alt="">
</figure> 

<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/ssets/post_images/2019-09-22-Paper-Review-2-VDSR-Super-Resolution/Untitled-fc2f199c-011b-479e-8227-7d4d7f47831f.png" alt="">
</figure> 

## Valuable Relative Works

- [SRCNN](https://arxiv.org/pdf/1501.00092.pdf)
