# Red Light Running Detect System
### The 3rd Chungnam National University-PURDUE University
### Jr. Capstone Design
-------------------------------------------------------

## Red Light Running(RLR)
```
신호등이 빨간색으로 바뀐 후 차량이 멈춰야 함에도 불구하고 운전자가 신호를 위반하는 행동
```

-------------------------------------------------------

## 프로젝트 목표
```
교차로에 Laser Pointer와 LED를 이용하여 운전자가 RLR 차량을 인식할 수 있도록 하는 것
```

-------------------------------------------------------


## 사용한 센서
```
1. LIDAR SENSOR - LIDAR Lite v3
2. RADAR SENSOR - HB 100
```

-------------------------------------------------------


## 작동 원리
```
Lidar sensor로 정지선을 향해 오는 차량의 속도를 측정

Radar sensor로 센서와 차량 사이의 거리를 측정

측정된 속도와 거리를 아두이노로 전송

아두이노에서는 Stopping Sight Distance(SSD)를 구할 수 있도록 의미 있는 데이터 값만 추출

얻어진 SSD 값을 이용하여 Laser pointer와 LED가 교차로에 쏘아져야 할 각도를 구함
```
