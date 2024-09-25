---
layout: page
title: Remote control
subtitle: Smart mobilities & Motor design & Autonomous-driving
---

# Remote control (원격 제어 시스템)
저희랩에서는 모빌리티 전반의 원격제어 시스템에 관한 연구를 진행하고 있습니다

---

## Core Idea #1 : 원격제어를 사용한 실 차량제어

**5G/LTE 망을 사용한 국내 유일의 양방향 원격 관제센터 개설**

![labpic](https://github.com/hrchalab/hrchalab.github.io/blob/master/assets/remote/원격제어영상1.gif?raw=true){: width="850" height="400"}

![labpic](https://github.com/hrchalab/hrchalab.github.io/blob/master/assets/remote/원격제어영상2.gif?raw=true){: width="850" height="400"}
> (전국 유일의 양방향 관제센터) 광주광역시 한국생산기술연구원 서남본부 소재

- 2019년부터 광주무인저속특장차 규제자유특구 사업을 통해 총합 700시간, 1,700여 km를 관제중에 있음

![](https://github.com/hrchalab/hrchalab.github.io/blob/master/assets/remote/EV.JPG?raw=true)
> (원천차량) 1.5T 급의 무인자율주행 차량을 사용한 실 원격제어 구성

---

## Core Idea #2 : 무선 원격제어의 통신지연 양상 분석

**원격주행 테스트를 통한 실제 통신지연의 프로필 (Communication delay profile)을 조사**
![labpic](https://github.com/hrchalab/hrchalab.github.io/blob/master/assets/remote/communication_delay.png?raw=true)
> Gaussian Mixture Model (GMM)을 사용한 통신 지연의 모델링

![labpic](https://github.com/hrchalab/hrchalab.github.io/blob/master/assets/remote/example_teleopration.png?raw=true)
> 양방향 통합 관제센터의 구성

![labpic](https://github.com/hrchalab/hrchalab.github.io/blob/master/assets/remote/GPS.png?raw=true)
> GPS 의 PPS 신호를 활용한 나노초 단위의 시간동기를 통해 단방향 통신지연시간을 계측

![labpic](https://github.com/hrchalab/hrchalab.github.io/blob/master/assets/remote/experiment.jpg?raw=true)
> 실차량 및 통합관제센터간의 통신구성도

![labpic](https://github.com/hrchalab/hrchalab.github.io/blob/master/assets/remote/profile.jpg?raw=true)
> 초저지연 양방향 관제센터와 대상차량간의 단방향 통신지연 계측 결과 및 프로필 생성

## Core Idea #3 : 단방향 통신지연의 보상을 통한 원격제어 성능의 향상

**통신지연 보상기의 설계를 통한 미래제어명령 예측자 설계**
![labpic](https://github.com/hrchalab/hrchalab.github.io/blob/master/assets/remote/mechanism.jpg?raw=true)
> 무향 칼만필터를 기본으로하여 단방향 통신지연만큼의 예측기설계를 통해 실제 수신값과의 확률적 보상

![labpic](https://github.com/hrchalab/hrchalab.github.io/blob/master/assets/remote/result.jpg?raw=true)
> 일정한 통신지연 뿐만이 아니라, 일시적인 통신두절이나, 단발적이상값에 대한 내성이 강화되고, 성능의 향상을 확인

**인공신경망을 사용한 미래제어명령/영상정보 예측기 설계**
![labpic](https://github.com/hrchalab/hrchalab.github.io/blob/master/assets/remote/pLSTM.png?raw=true)
> 시계열 예측에 좋은 LSTM을 활용한 통신지연 보상기의 설계

![labpic](https://github.com/hrchalab/hrchalab.github.io/blob/master/assets/remote/predictor.png?raw=true)
> 시계열예측에 좋은 LSTM과 영상활용에 뛰어난 CNN 을 활용한 시계열 영상 예측기 설계

![labpic](https://github.com/hrchalab/hrchalab.github.io/blob/master/assets/remote/convlstm.gif?raw=true)
> 시뮬레이터를 활용한 영상예측 결과 비교영상 (좌:지연, 중:보상, 우:실제)

---

**Author: Eugene Kim**
