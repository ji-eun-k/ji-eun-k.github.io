---
title: "epoch와 batch size, iteration"
tags :
toc: true
toc_sticky : true
use_math : true
---


## epoch

**전체 데이터 셋을 반복하는 횟수**

전체 데이터셋으로 forwardpropagation(순전파)와 backwardpropagation(역전파)가 완료되면 1번의 epoch가 진행되었다고 보면된다.

반복적인 학습을 통해 높은 정확도의 모델을 만들 수 있다.

<br>

💡 설정한 epoch 값이 너무 작다면 underfitting, 너무 크다면 overfitting이 발생할 확률이 높아짐 <br>


## batch size
**한번에 학습할 데이터의 수**

<br>

💡 메모리의 한계와 속도 저하 때문에 한 번의 epoch에서 모든 데이터를 한꺼번에 집어넣을 수 없음 <br>

## interation
**한 epoch 에서 batch를 학습하는 횟수**

전체 데이터에 대한 오차 총합으로 propagation을 수행하면 weight가 한 번에 크게 변할 수 있기 때문에 gradient decent처럼 조금씩 이동해 최적화 할 수 있도록 한다.<br>


💡 데이터가 100개, batch size가 10 이면, 1 Epoch = 10 iteration