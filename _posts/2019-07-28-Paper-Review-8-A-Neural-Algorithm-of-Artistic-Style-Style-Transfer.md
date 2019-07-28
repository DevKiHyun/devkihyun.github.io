---
title: "Paper Review 8 - A Neural Algorithm of Artistic Style [Style Transfer]"
categories:
  - study
tags:
  - deep learning
  - Style Transfer
  - Representation
last_modified_at: 2019-07-28T22:00:00+09:00
comments: true
mathjax: true
sitemap :
  changefreq : daily
  priority : 1.0
---

# [A Neural Algorithm of Artistic Style](https://arxiv.org/pdf/1508.06576.pdf)

- Accepted Conference Name & Year : CVPR, 2016 - **[Image Style Transfer Using Convolutional Neural Networks](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Gatys_Image_Style_Transfer_CVPR_2016_paper.pdf)**
- 1st Author Name & Institute : Leon A. Gatys, University of Tubingen

## Contribution

- 이전의 [[Understanding Deep Image Representations by Inverting Them](https://arxiv.org/pdf/1412.0035.pdf)] 에서 이미지의 feature 으로부터 이미지를 복원이 가능한 것을 확인할 수 있다.
- 원본 이미지의 content 를 reconstruct 하면서 동시에 style 을 제공하는 이미지의 feature 와도 같아지게끔 reconstruct 하면 어떻게 될지를 잘 보여주는 정말 인상 깊은 논문이다.
- 각각의 reconstruct loss 를 결합한 것 뿐이기 때문에 심플한 구조가 장점이다.
- 기본적으로 이미지의 feature 를 extraction 하기 위해서 기존의 State of the Art 한 CNN 모델을 pretrained 모델로 사용한다. 본 논문에선 VGG19를 사용했다.

## Comments

- 직접 구현하면서 알게 된 점은 오픈소스에 공개된 pretrained model들의 가중치가 동일한 것이 아니기 때문에 각 모델에서 extraction 된 이미지의 feature가 전부 동일한 값을 갖고 있다고 할 수 없다. 이런 부분이 style transfer 의 결과에 어느정도 영향을 주기도 한다. 따라서 결과가 이상하게 나온다면 pretrained model을 다른 오픈소스를 사용해보는 것을 추천한다. (Keras 에서 offical 로 제공하는 VGG는 VGG19 보단 VGG16을 쓰는것이 좋다.)
- Style 이 너무 강한 경우엔 오히려 기괴한? 느낌을 주는 결과를 내보내기도 한다.

## Proposed Architecture
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-07-28-Paper-Review-8-A-Neural-Algorithm-of-Artistic-Style-Style-Transfer/Untitled-3e30849e-9a4c-42b8-b0e3-a0e55aa17d89.png" alt="">
</figure> 
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-07-28-Paper-Review-8-A-Neural-Algorithm-of-Artistic-Style-Style-Transfer/Untitled-35087384-c873-485f-9400-6bb4c1cb79d9.png" alt="">
</figure>

## Dataset
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-07-28-Paper-Review-8-A-Neural-Algorithm-of-Artistic-Style-Style-Transfer/Untitled-7dde9b08-11a7-4ddb-a9ce-eab0a386512c.png" alt="">
</figure> 
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-07-28-Paper-Review-8-A-Neural-Algorithm-of-Artistic-Style-Style-Transfer/Untitled-4ec4ad2f-662d-4aa5-ab05-406cefedda0c.png" alt="">
</figure>
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-07-28-Paper-Review-8-A-Neural-Algorithm-of-Artistic-Style-Style-Transfer/Untitled-ac270b0f-1b3a-407e-89ba-eeaec1785e79.png" alt="">
</figure>
