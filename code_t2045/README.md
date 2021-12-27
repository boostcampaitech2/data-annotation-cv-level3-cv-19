# Data Annotation Project

# 파일 구성
1. board2_make_train_json.ipynb
    - 캠퍼들과 함께 제작한 annotation 결과물은 polygon 형태의 annotation도 포함이 되어 있음
    - polygon 형태의 annotation을 사각형 형태로 분리하여 json 파일 형태로 저장함. 이제 EAST Model에 적용 가능

2. dataset.py
    - 기본 Dataset에, 캠퍼들과 함께 제작한 데이타를 추가

3. train.py
    - argument에 캠퍼들과 함께 제작한 테이타의 경로를 받을 수 있도록 추가

  
# 결과 변화
  - 기본 Dataset에 캠퍼들과 같이 제작한 annotation 결과물을 추가하였다. 
  - noise가 많이 있었지만, 적용 후에 Score가 대폭 향상되었다. 

| 적용전     | 적용전  | 적용후 |
| --------- | --------|--------| 
| F1        | 0.4825  | 0.5659 |
| Recall    | 0.3821  | 0.4476 |
| Precision | 0.6545  | 0.7693 |

  

