# Paper Review 5 - EDSR [Super Resolution]

# [Enhanced Deep Residual Networks for Single Image Super-Resolution](https://arxiv.org/pdf/1707.02921v1.pdf)

- Accepted Conference Name & Year : CVPR 2017
- 1st Author Name & Institute : Bee Lim, Seoul National University

## Contribution

- Residul block 을 사용하지만 resnet 과 달리 Batch Normalization, Relu(residula block의 outside) 을 제거하고 더 깊은 residual block 을 쌓아 뛰어난 성능을 보여줌.
- 기존의 SR 들은 L2 loss(MSE)를 주로 사용했지만 L1 loss 를 사용해도 좋은 결과가 나온다는 것을 보여줌.
- Single-Scale 과 Multi-Scale 두 가지의 모델을 제시함.

## Proposed Architecture

![](Untitled-1cdff0f9-1ddc-45ca-ac23-8b8981d74545.png)

![](Untitled-52fb0b7e-4aa4-4895-8ba3-dfe6a0b1fda7.png)

![](Untitled-d3b4bdc6-96d0-4229-8aae-f63843f82c46.png)

## Dataset

![](Untitled-d70c90d1-4909-49b0-bea2-7668bb691082.png)

![](Untitled-885f26ef-1b00-4f2a-baa7-e145c00fa38c.png)

![](Untitled-b5bdce8a-18a5-4a41-bf1c-7c5985421ceb.png)

## Valuable Relative Works

- SRResnet
- [ESPCN](https://arxiv.org/pdf/1609.05158)