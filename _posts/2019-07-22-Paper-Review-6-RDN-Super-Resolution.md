---
title: "Paper Review 6 - RDN [Super Resolution]"
categories:
  - study
tags:
  - deep learning
  - Super Resolution
last_modified_at: 2019-07-22T23:25:00+09:00
comments: true
mathjax: true
sitemap :
  changefreq : daily
  priority : 1.0
---

# [Residual Dense Network for Image Super-Resolution](https://arxiv.org/pdf/1802.08797.pdf)

- Accepted Conference Name & Year : CVPR 2018
- 1st Author Name & Institute : Yulun Zhang, Northeastern University

## Contribution

- 기존의 SR 들은 resnet 의 구조 덕에 더욱 깊은 학습이 가능해졌지만 깊어진 layer 들의 정보를 충분히 활용하지 못하는 점이 있다.
- Densenet 의 구조를 채용해 선행 features 을 다음 layer에도 concatenate 로 직접 전달 할 수 있게  되면서 아주 좋은 결과를 보여줬다.
- 학습 시 just bicubic, blur, gaussian noise 세 가지 방식으로 input 데이터를 처리하는 실험을 진행해 자세한 결과를 나타냈다.

## Proposed Architecture
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-07-22-Paper-Review-6-RDN-Super-Resolution/Untitled-018cead3-42c7-4735-b3ec-a0fd763791e1.png" alt="">
</figure> 
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-07-22-Paper-Review-6-RDN-Super-Resolution/Untitled-8cae05a5-af63-4f9b-93b8-08fc1ca33042.png" alt="">
</figure> 

## Dataset
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-07-22-Paper-Review-6-RDN-Super-Resolution/Untitled-f7917cf6-84e1-42e5-9757-812c2adb89ac.png" alt="">
</figure> 
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-07-22-Paper-Review-6-RDN-Super-Resolution/Untitled-3e21e98d-f9aa-4704-b1be-84e1f645f048.png" alt="">
</figure>
<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2019-07-22-Paper-Review-6-RDN-Super-Resolution/Untitled-22fc337b-9675-48b4-87f8-18c76d9d1c3f.png" alt="">
</figure> 

## Valuable Relative Works

- [Resnet](https://arxiv.org/pdf/1512.03385.pdf)
- [Denenet](https://arxiv.org/pdf/1608.06993.pdf)
- [ESPCN](https://arxiv.org/pdf/1609.05158.pdf)
