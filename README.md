Image 10 classifier
# 성능 향상 기법들
1. underfitting 방지

* 데이터 증강 (오히려 성능을 저하 시켰음)
* lr 학습률 조절(0.001 > 0.005)
* lr 이 성능에 가장 크게 영향을 줘서 lrscheduler 사용 (절반씩 감소하게 세팅)
* Con2D, maxPooling 계층 추가
* 뉴런 수를 각 레이어에 자연스럽게 크기 맞춤 

2. Overfitting 방지

* Dropout, Batch Normalization 사용 (언더 피팅 확인, dropout 비율 조정)
* 이미지 퀄리티가 높아져서 배운 기법들과 과정으로는 오버피팅 까지는 안 나오는 것 같습니다