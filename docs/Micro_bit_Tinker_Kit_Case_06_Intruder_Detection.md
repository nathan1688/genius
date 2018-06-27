![](https://i.imgur.com/beCyIpm.png)
도둑질은 안되!
이 간단한 침입자 탐지 시스템으로 도둑을 그만 두십시오.


## 단계 0 - 사전 빌드 개요
---

이 프로젝트에서 우리는 누군가가 문을 열 때 소리를 낼 침입자 탐지 시스템을 만들 것입니다. 집의 상태가 OLED에 표시됩니다.


## 재료 :
---

- 1 x [BBC 마이크로 : 비트] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 마이크로 USB 케이블 1 개
- 1 x [브레이크 아웃 보드] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 x [Crash Sensor] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 x [OLED] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 x [Buzzer] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 2 x 암 - female 점퍼 선


목표 :
---

- 충돌 센서, OLED 및 부저에 대해 알아보십시오.
- OLED로 무언가를 만들어라.
- 충돌 센서로 무언가를 만드십시오.


## 만드는 방법
---

### 1 단계 - 구성 요소

마이크로 비트를 브레이크 아웃 보드에 삽입하고 마이크로 USB 케이블을 연결하십시오.

![](https://i.imgur.com/cvJnbqE.jpg)  

그런 다음 점퍼 케이블을 사용하여 버저를 핀 0에 연결하십시오. 아래 그림과 같이 OLED를 연결하십시오. 세 행 중 하나에 플러그를 연결할 수 있어야합니다.

![](https://i.imgur.com/3benydL.jpg)  

충돌 센서를 핀 1에 연결하십시오. 와이어의 색상이 브레이크 아웃 보드의 색상 핀과 일치하는지 확인하십시오. 

![](https://i.imgur.com/YvQkd81.jpg)  

### 2 단계 - 사전 코딩

![](https://i.imgur.com/qPgEmnW.jpg)  

우리는 키트 구성 요소를 사용할 수 있도록 코드 패키지를 추가 할 것입니다. 코드 드로어에서 고급을 클릭하면 더 많은 코드 섹션을 볼 수 있고 패키지 추가를위한 코드 드로어의 하단을 볼 수 있습니다.

![](https://i.imgur.com/IWhPZeP.png)  

그러면 대화 상자가 열립니다. "팅커 키트"를 검색 한 다음이 패키지를 다운로드하려면 클릭하십시오.

![](https://i.imgur.com/b0vriWO.png)  

참고 : 비 호환성 문제로 인해 일부 패키지가 제거된다는 경고 메시지가 표시되면 프로젝트 파일 메뉴에서 프롬프트를 따르거나 새 프로젝트를 만듭니다.

### 3 단계 - 코딩

![](https://i.imgur.com/OKjXb0c.jpg)  

코드 드로어 안의 Tinkercademy를 ​​클릭하면 키트의 다양한 구성 요소에 대한 맞춤 블록을 찾을 수 있습니다.

![](https://i.imgur.com/UwHfSVv.jpg)  

처음에는 항상 OLED를 초기화해야합니다. 64 및 128은 각각 OLED의 높이 및 폭을 나타낸다.

![](https://i.imgur.com/GIhLCLU.jpg)  

두 가지 조건 만 있으므로 "else-if"문 하나만 있으면됩니다.
충돌 센서가 트리거되면 버저가 울리고 OLED에 "침입자 감지 됨"메시지가 표시됩니다. 그렇지 않으면 크래시 센서에 힘이 가해지지 않으면 부저가 울리지 않고 OLED는 "집은 안전합니다"라는 메시지를 표시합니다.

이 코드를 직접 입력하지 않으려면 
[https://makecode.microbit.org/_A0zFxqMPMXbo](https://makecode.microbit.org/_A0zFxqMPMXbo)

또는 아래 페이지에서 다운로드 할 수 있습니다.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_A0zFxqMPMXbo" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### 4 단계 - 성공!

올레! 당신은 침입자 탐지기를 만들었습니다!
