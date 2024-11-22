# 신경망 층별 실험 

## 실행 방법 및 실험 안내

### 환경 설정

신경망 학습 및 실행을 위해 아래 패키지 설치가 필요합니다:

- `numpy`
- `matplotlib`
- `tensorflow`

터미널에서 다음 명령어를 실행하세요:

```bash
pip install numpy matplotlib tensorflow
```

---

### 코드 실행 순서

아래 명령어를 통해 각 신경망 실험을 실행할 수 있습니다:

- **2층 신경망**: `python train/train_two_layer_net.py`
- **3층 신경망**: `python train/train_three_layer_net.py`
- **4층 신경망**: `python train/train_four_layer_net.py`
- **5층 신경망**: `python train/train_five_layer_net.py`

---

### 각 신경망의 구조

- **2층 신경망**: 입력(784) → 은닉층(50) → 출력(10)
- **3층 신경망**: 입력(784) → 은닉1(100) → 은닉2(50) → 출력(10)
- **4층 신경망**: 입력(784) → 은닉1(100) → 은닉2(80) → 은닉3(60) → 출력(10)
- **5층 신경망**: 입력(784) → 은닉1(100) → 은닉2(80) → 은닉3(60) → 은닉4(40) → 출력(10)

---

### 결과 확인 방법

각 실험이 끝난 후 두 개의 그래프가 표시됩니다:

1. **위쪽 그래프**: 전체 정확도 범위(0~1.0)
2. **아래쪽 그래프**: 높은 정확도 구간(0.9~1.0) 확대

---

### 관찰할 점

1. **학습 속도**: 각 모델이 높은 정확도에 도달하는 속도
2. **최종 정확도**: 각 모델의 최종 성능
3. **과적합 여부**: 훈련 정확도와 테스트 정확도의 차이
4. **안정성**: 학습 곡선의 안정성

---

### 실험 결과 기록 방법

각 모델의 실행이 끝난 후 다음을 기록하세요:

- **최종 훈련 정확도**
- **최종 테스트 정확도**
- **학습에 걸린 시간**
- **특이사항** (불안정한 학습, 과적합 등)

---

### 주의사항

1. 모든 실험은 **동일한 조건**에서 진행됩니다:

   - 에폭 수: `100`
   - 배치 크기: `100`
   - 학습률: `0.1`

2. 랜덤 초기화로 인해 실행할 때마다 결과가 약간 달라질 수 있습니다.

---

## 실험 목적

신경망의 층이 깊어질수록:

1. **학습 능력이 향상되는가?**
2. **학습 시간이 얼마나 증가하는가?**
3. **과적합이 발생하는가?**

이 실험을 통해 신경망의 **깊이가 학습에 미치는 영향**을 직접 관찰할 수 있습니다.
```
