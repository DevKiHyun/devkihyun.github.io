# Paper Review 9 - FARED [Anomaly Detection]

# [Fast Adaptive RNN Encoder–Decoder for Anomaly Detection in SMD Assembly Machine](https://www.mdpi.com/1424-8220/18/10/3573)

- 1st Author Name & Institute : YeongHyeon Park, Department of Computer and Electronic Systems Engineering, Hankuk University of Foreign Studies

## Contribution

- 제품을 조립하는 기계소리만 가지고서 정상/비정상인지를 판단하는 Anomaly Detection 연구이다.
- 본 논문에서는 실제 현상에서 다양한 기계들이 조립하고 제품 변경이 이루어지기 때문에 시간적여유가 없는 상황에서도 충분히 대응할 수 있는 rnn 기반의 Anomaly Detection 을 선보임.
- 정상적인 소리만 가지고서 입력한 뒤 다시 입력과 동일한 출력이 나오도록 학습 시킨다. 뿐만 아니라 최대한 정상적인 소리에 대해서만 오버피팅이 잘 되도록 한다. 그러면 비정상적인 소리가 들어올 경우 제대로 복원이 되지 않기 때문에 복원 정도에 대한 오차로 정상/비정상을 판단 할 수 있게된다.

## Proposed Architecture

![](Untitled-21fb0f8f-0d52-4428-a2c8-ef8c4362d809.png)

![](Untitled-18f7bb3c-bbfa-408d-a7e6-d727eb643147.png)

## Dataset

![](Untitled-42bfc58b-418b-4676-bf45-8a00485eb655.png)

![](Untitled-04987144-d5e7-48db-91e3-969cd7b2e4f2.png)

![](Untitled-6f617184-4df0-4f34-b2e1-fe2676806298.png)

## Valuable Relative Works

- [Residual Error Based Anomaly Detection Using Auto-Encoder in SMD Machine Sound](https://www.mdpi.com/1424-8220/18/5/1308)