# 자동차 차체 유형 인식 모델🚗

<br>

이 프로젝트는 다양한 자동차 차체 유형을 인식하는 강력한 머신러닝/딥러닝 모델을 개발하는 것을 목표로 합니다. 
사용된 데이터셋은 Convertible, Coupe, Hatchback, Pick-Up, SUV, Sedan, VAN과 같은 7가지 차체 유형의 이미지로 구성되어 있습니다.

<br>

## 데이터셋 개요
- **총 클래스 수:** 7
- **클래스 명:** Convertible, Coupe, Hatchback, Pick-Up, SUV, Sedan, VAN
- **총 이미지 수:** 7,000 (각 클래스당 1,000개의 이미지)

<br>

## 모델 아키텍처
- **사전 훈련된 모델:** DenseNet121
- **Dense 블록 수:** 4
- **레이어 수:** 121

<br>

## 하이퍼파라미터 및 훈련 설정
- **학습률:** 0.001
- **배치 크기:** 64
- **에폭 수:** 50

<br>

## 최적화 전략
훈련 도중 다양한 최적화 알고리즘을 실험하여 이 작업에 가장 적합한 것을 찾았습니다.

## 학습률 조절
학습률을 조절하여 모델 수렴과 성능을 향상시켰습니다.

## 모델 복잡성 조절
DenseNet121 모델의 복잡성을 조절하여 과소적합과 과적합 사이의 균형을 유지했습니다.

## 배치 크기 조절
다양한 배치 크기를 테스트하여 모델 훈련 및 성능에 미치는 영향을 조사했습니다.

<br>

## 최종 성능
50 에폭의 훈련 후, 모델은 다음과 같은 성능을 달성했습니다:

- **훈련 손실:** 0.5580, **훈련 정확도:** 80.67%
- **검증 손실:** 6.1670, **검증 정확도:** 2.85%
