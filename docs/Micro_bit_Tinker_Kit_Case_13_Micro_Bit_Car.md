내가 만들어 스스로 운전하는 자기 운전 마이크로 : 비트 차를 만들어라!
(주의 : 언덕을 굴러 다니는 공이 "자가 운전"이기만하면 "자가 운전"일뿐입니다.)

## 목표
---

-이 프로젝트에서 우리는 Micro : bit, Breakout Board 및 Servos를 사용하여 자가 운전하는 자동차를 만듭니다!
- Servo 및 Micro : bit, Breakout Board 및 MakeCode와 함께 사용하는 방법에 대해 알아보십시오.
-이 일이 얼마나 웃긴지 놀라워!

노트 :
이 활동은 팅커 키트에없는 추가 부품을 사용합니다.
(우리의 차량용 키트 온라인 스토어에서 계속 지켜봐주십시오!)


## 재료
---
- 1 x BBC 마이크로 : 조금
- 마이크로 USB 케이블 1 개
- 1 x 배터리 상자
- AA 배터리 2 개
- 1 x 브레이크 아웃 보드
- 2 x 서보
- 1 x 아크릴 자동차 바디
- 2 x 바퀴
- 1 x 펠트 패드
- 끈적한 테이프

![](http://www.elecfreaks.com/estore/download/microbit-car-1.jpg)  
![](http://www.elecfreaks.com/estore/download/microbit-car-2.jpg)  

## 만드는 방법
---

### 1 단계

다음 그림과 같이 자동차 부품을 연결하십시오.
자동차 키트를 사용하는 경우 차체의 레이블을 따라 끈끈한 테이프로 부품을 올바르게 삽입하십시오.
서보 커넥터를 브레이크 아웃 보드의 핀 0과 핀 1에 연결하십시오.
일반 서보 케이블의 색상은 브레이크 아웃 보드의 노란색, 빨간색 및 검정색 구성표와 정확하게 일치하지 않습니다. 주황색 서보 케이블을 노란색 핀에 연결하고 갈색 서보 케이블을 검정색 핀에 연결하십시오.

![](http://www.elecfreaks.com/estore/download/microbit-car-3.jpg)  
![](http://www.elecfreaks.com/estore/download/microbit-car-4.jpg)  
![](http://www.elecfreaks.com/estore/download/microbit-car-5.jpg)  
![](http://www.elecfreaks.com/estore/download/microbit-car-6.jpg)  

### 2 단계

표시된 블록을 시작 블록에 추가하십시오.
이게 뭐야? 시작할 때마다 고정 위치로 서보를 리셋하십시오!
MakeCode의 Servo 블록 (빨간색으로 표시됨)은 0에서 180까지의 값을가집니다. 고급, 핀 다음에서 찾을 수 있습니다.
우리가 사용하고있는 연속적인 서보의 경우 중간 값이 90입니다. 다른 말로하면, 우리는 서보에게 "여전히"있다고 말하고 있습니다.
이미지를 표시하여 Micro : bit에 코드를 다운로드했음을 시각적으로 나타냅니다.

### 3 단계

바퀴를 움직이자! 오른쪽에 표시된 코드를 Forever 블록에 추가하십시오.
Digital Write Pin to 0 블록은 Advanced, Pins 아래에도 있습니다.
여기 무슨 일 이니? 하나의 서보를 시계 방향 (180도)으로 돌리고 다른 서보는 끕니다. 그런 다음 잠깐 멈춘 후에 이전 서보를 끄고 서보를 반 시계 방향 (0)으로 돌립니다. 기억하십시오, 90 곧장입니다!
왜 우리는 한 번에 하나의 servo를 꺼야합니까? 이는 배터리 전원 요구 사항 때문입니다. 마이크로 비트는 한 번에 두 서보 전원에 문제가 있습니다. 관심이 있다면 외부 전원이있는 DC 모터를 사용하여 탐색 할 수 있습니다. 아니면 이메일로 더 자세한 정보를 얻을 수 있습니다!
모터가 올바른 방향을 향하고 있는지 확인하십시오. 0과 180 값을 바꿔 모터의 이동 방향을 변경할 수 있습니다.

![](http://www.elecfreaks.com/estore/download/microbit-car-7.jpg)  

이 코드를 직접 입력하지 않으려면 아래 링크에서 직접 다운로드 할 수 있습니다.

[https://makecode.microbit.org/_Ef87EJAepcve](https://makecode.microbit.org/_Ef87EJAepcve)  

또는 아래 페이지에서 다운로드 할 수 있습니다.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_Ef87EJAepcve" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### 성공!
자동차를 운전할 준비가되면 배터리 팩을 마이크로 비트에 연결하면 자동차가 작동합니다. 게다가 공기 역학적 인 특성을 향상시키기 위해 공예 재료로 차를 튜닝 할 수 있습니다! 추가 확장을 위해 자동차를 자율적으로 움직이는 대신 수동으로 모터를 제어하는 ​​ADKeyboard를 연결할 수도 있습니다.

![](http://www.elecfreaks.com/estore/download/microbit-car-8.jpg)  
![](http://www.elecfreaks.com/estore/download/microbit-car-9.jpg)  
![](http://www.elecfreaks.com/estore/download/microbit-car-10.jpg)  


