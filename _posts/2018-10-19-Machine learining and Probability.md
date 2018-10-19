---
title: "머신러닝과 확률"
categories:
  - study
tags:
  - probability
  - statics
  - machine learning
  - deep learning
last_modified_at: 2018-10-19T14:27:00+09:00
comments : true

gallery_1:
  - url: /assets/post_images/2018-10-19-Machine_learning_and_Probability/0.PNG
    image_path: /assets/post_images/2018-10-19-Machine_learning_and_Probability/0.PNG
    title: "Explain neural network"
---

안녕하세요. 이번 시간에는 머신러닝과 확률을 얘기하려고 합니다. 최소한 [모두의 딥러닝](https://hunkim.github.io/ml/) 강의를 이수한 수준은 필요로 하고 기본적으로 고등학교 수준의 확률과 통계를 알고 있다고 여기고 진행하겠습니다.


# 확률론적 관점

최근엔 잘 만들어진 딥러닝 프레임워크들이 많아 코딩만 할 줄 알면 딥러닝에 대해 깊이 있게 몰라도 데이터와 코드 몇 줄만으로도 그럴듯한 결과물을 얻을 수 가 있습니다. 그래서 딥러닝 개발의 진입 장벽이 많이 낮아졌다고 할 수 있죠. 그 과정에서 선형대수에 관련된 문서나 글을 읽을 일이 많아 선형대수가 중요하다는 것은 알겠는데, 확률과 통계는 그럼 진짜 중요한가? 하는 의문이 들기도 합니다. 중요하다는 얘기는 많이 들었는데 정작 체감을 못하기 때문입니다. 그래서 이번엔 우리가 알고 있는 딥러닝 모델을 확률론적인 관점에서 해석해보고자 합니다.

__분류 문제(Classification)__ 를 예시로 한번 들어보겠습니다. 우리가 딥러닝으로는 제일 먼저 해보게 되는게 아마 __MNIST 숫자 손글씨 데이터__ 로 해당 숫자를 분류해보는 과제일겁니다. MNIST는 __숫자 데이터 X와 클래스 Y(라벨)가 쌍으로 구성된 데이터셋__ 입니다. 단순하게 베이직한 뉴럴네트워크로 이루어져 있는 모델이 있다고 하면, 우리가 입력 값으로 X를 넣으면, 모델이 계산한 결과(Output)를 Y랑 비교하면서 잘 분류가 되도록 학습됩니다. 즉, 이 모델은 데이터 X를 잘 이해해서 해당 클래스 Y를 *'예측'* 할 수 있는 *'함수'* 를 알아내는 겁니다. 보통은 이 학습과정을 선형대수로도 충분히 설명을 할 수 있습니다. 지금까지 설명한 내용을 아래의 그림으로 간단히 나타낼 수 있습니다.

<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/post_images/2018-10-19-Machine_learning_and_Probability/0.PNG" alt="">
  <figcaption>그림출처 http://sanghyukchun.github.io/58/</figcaption>
</figure> 

