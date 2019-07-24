---
title: "Paper Review 7 - Invert CNN [Invert Representation]"
categories:
  - study
tags:
  - deep learning
  - Visualizaion
  - Representation
last_modified_at: 2019-07-22T23:21:00+09:00
comments: true
mathjax: true
sitemap :
  changefreq : daily
  priority : 1.0
---

# [Understanding Deep Image Representations by Inverting Them](https://arxiv.org/pdf/1412.0035.pdf)

- Accepted Conference Name & Year : CVPR 2015
- 1st Author Name & Institute : Aravindh Mahendran, University of Oxford

## Contribution

- Convolutional Network의 중간 feature 를 통해서 다시 이미지를 복원해보는 실험으로 일종의 Visualization 이다.
- Content image 와 Random noise image 를 넣고 Content image 의 feature 에 가까워지도록 Random noise image 를 업데이트 시키는 방식으로 해서 Network 의 parameters 가 아닌 image 를 업데이트 하는 방식으로 진행된다.
- Features 를 통해 원본 데이터를 control 할 수 있다는 영감을 준다.

## Proposed Architecture

논문에는 존재하지 않아 Style Transfer 에 사용된 네트워크의 사진을 첨부한다.  원리는 동일하다. 직관적인 그림으로 이해하기 쉬울 것이다.

<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-09-22-Paper-Review-7-Invert-CNN-Invert-Representation/Untitled-35087384-c873-485f-9400-6bb4c1cb79d9.png" alt="">
</figure> 

## Dataset
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-09-22-Paper-Review-7-Invert-CNN-Invert-Representation/Untitled-8eeae7c0-ab10-479f-b7b9-d11b0cf1bc55.png" alt="">
</figure> 
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-09-22-Paper-Review-7-Invert-CNN-Invert-Representation/Untitled-9577190e-5d7b-4d14-b430-11fd5879ed63.png" alt="">
</figure> 
