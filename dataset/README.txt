데이터세트 설명
딥러닝 모델을 학습하기 위한 데이터세트입니다.
* 하나의 냉장고에서 수집
* 상온, 냉동고, 냉장고에서 온습도 데이터 수집
* 주기적으로 냉장고, 냉동고의 문을 10초간 열고 닫는 방식으로 데이터 수집
* 5초 간격으로 데이터를 수집(실제 제품은 1분 간격으로 수집되므로 학습 시 적절하게 세그먼트를 생성)
* 데이터세트의 컬럼은 다음과 같습니다.(상온 온도/상온 습도/냉동고 온도/냉동고 습도/냉장고 온도/냉장고 습도/Ground Truth)
* Ground Truth 라벨링은 (냉장고 문 열림:1, 냉동고 문 열림:2, 냉장고/냉동고 문 열림:3)입니다.

딥러닝 학습(~.ipynb)
* google colab을 이용
* 냉장고의 문열림이나 냉동고의 문열림을 따로 학습하기 위해서 둘 중 하나의 데이터를 지우고 입력
* 세가지의 복잡도를 가지는 딥러닝 모델을 이용해서 학습 및 결과 출력