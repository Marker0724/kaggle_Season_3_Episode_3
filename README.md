# Sk Shieldus Rookies 머신러닝 미니 프로젝트 (5조)

## Kaggle Season 3, Episode 3

- 실행 환경
  - Google Colab
  - Python 3.8.10
  - Sklearn 1.2.1
  - CatBoost 1.1.1
 
- Blending 시, Colab 기본 환경 사용 (Sklearn 업데이트 X)

---

# 목표
- **0.897 넘기기 (10%(66등) 안에 들기)**

---


# 데이터 준비

```
import numpy as np
import pandas as pd

# 데이터 경로
data_path = '/content/'

train = pd.read_csv(data_path + 'train.csv',index_col='id')
test = pd.read_csv(data_path + 'test.csv',index_col='id')
submission = pd.read_csv(data_path + 'sample_submission.csv',index_col='id')

# 다운받아서 불러옴
ibm = pd.read_csv(data_path + 'WA_Fn-UseC_-HR-Employee-Attrition.csv')
ibm.head(2)
```

- 모델 성능 향상 데이터 추가
- https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

