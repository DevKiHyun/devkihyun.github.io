---
title: "Paper Review 3 - ESPCN [Super Resolution]"
categories:
  - study
tags:
  - deep learning
  - Super Resolution
last_modified_at: 2019-07-22T22:58:00+09:00
mathjax: true
sitemap :
  changefreq : daily
  priority : 1.0
---

# [Real-Time Single Image and Video Super-Resolution Using an Efficient Sub-Pixel Convolutional Neural Network](https://arxiv.org/pdf/1609.05158.pdf)

- Accepted Conference Name & Year : CVPR 2016
- 1st Author Name & Institute : Wenzhe Shi, Twitter

## Contribution

- 기존의 Deep Learning 을 적용한 SR 기법들은 Upsampling 단계 없이 입력 LR 이미지의 크기를 HR 해상도에 맞춰두고 진행하기 때문에 높은 계산량을 요구했다.
- 이번 논문은 입력 LR 이미지 크기를 늘리거나 또는 모델 단계에서 명시적인 upscaling layer 를 학습 할 필요없이 feature maps 에서 픽셀들을 뽑아 HR 이미지로 upscaling을 해주기 때문에 연산량을 줄일 수 있다.

## Proposed Architecture
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-09-22-Paper-Review-3-VDSR-Super-Resolution/Untitled-47cd65ff-bab1-4ca2-b49d-355a523ced61.png" alt="">
</figure> 
## Dataset
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-09-22-Paper-Review-3-VDSR-Super-Resolution/UUntitled-f8c68178-5254-40b4-b61d-7fa0315579a4.png" alt="">
</figure> 
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-09-22-Paper-Review-3-VDSR-Super-Resolution/UnUntitled-bf44d50c-3fe0-4381-b8fb-48eed7adf6af.png" alt="">
</figure> 

## Valuable Relative Works

- [SRCNN](https://arxiv.org/pdf/1501.00092.pdf)
- [VDSR](https://arxiv.org/pdf/1511.04587v2.pdf)
