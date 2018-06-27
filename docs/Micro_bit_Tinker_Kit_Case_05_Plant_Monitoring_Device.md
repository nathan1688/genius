![](https://i.imgur.com/kUZLoEo.jpg)

이 프로젝트에서는 물이 충분하지 않을 때 부저 소리가 나는 식물 모니터링을 만들 예정입니다.

수분 수준을 나타내는 메시지가 항상 OLED에 표시됩니다.


목표 :
---

1. 버저, OLED 및 습도 센서를 확인하십시오.
2. 수분 센서로 무언가를 만드십시오.


필요한 재료 :
---

- 1 x [BBC Micro : bit] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 x 마이크로 USB 케이블
- 1 x [Breakout Board] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 x [Mini Buzzer] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 x [OLED] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 x [수분 센서] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 2 x 암 - female 점퍼 전선

참고 : 구성 요소는 순서에 관계없이 연결할 수 있습니다.


## 만드는 방법
---

먼저, OLED를 연결하십시오.
세 행 중 하나에 플러그를 연결할 수 있습니다.
![](https://i.imgur.com/qOBV7Uf.png)  

P0에 버저를 연결하십시오. 와이어의 색상이 브레이크 아웃 보드의 핀 색상을 따르는 지 확인하십시오.

![](https://i.imgur.com/ABoiMrD.jpg)  

수분 센서를 P1에 연결하십시오.

![](https://i.imgur.com/jgTG7i6.jpg)  

더 많은 코드 섹션을 보려면 코드 드로어에서 고급을 클릭하십시오.
우리는 키트 구성 요소를 사용할 수있는 코드 패키지를 추가 할 것입니다.
"패키지 추가"에 대한 코드 드로어 하단을보고 클릭하십시오.

![](https://i.imgur.com/FOHSrAx.png)  

이 때 대화 상자가 나타납니다. 상자에 "tinker kit"를 검색 한 다음이 패키지를 다운로드하려면 "tinkercademy-tinker-kit"를 클릭하십시오.

![](https://i.imgur.com/G2nV10d.png)  

코드 드로어 안의 Tinkercademy를 ​​클릭하면 키트의 다양한 구성 요소에 대한 맞춤 블록을 찾을 수 있습니다.

![](https://i.imgur.com/57H4sCe.png)  
![](https://i.imgur.com/DaZC53n.png)  

그 후 Tinkercademy 섹션 아래의 블록을 사용하여 OLED를 초기화하십시오.

![](https://i.imgur.com/xAM8RDr.png)  

두 가지 조건 만 있으므로 "else-if"문 하나만 있으면됩니다.
마이크로 : 습도 센서의 값을 지속적으로 읽습니다.
수분 센서 값이 50 미만이면 냄비에 물이 충분하지 않음을 나타냅니다. 결과적으로 부저음이 울리고 "Water your plant"라는 메시지가 OLED에 표시됩니다. 그렇지 않으면 수분 센서 값이 50보다 크면 부저음이 울리며 OLED에 "공장 상태 양호"라는 메시지가 표시됩니다.

![](https://i.imgur.com/qy2wheV.png)  

이 코드를 직접 입력하지 않으려면 아래 링크에서 전체 프로그램을 다운로드 할 수 있습니다.
[https://makecode.microbit.org/_DV547gK8j9ms](https://makecode.microbit.org/_DV547gK8j9ms)  

또는이 페이지에서 다운로드 할 수 있습니다.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_DV547gK8j9ms" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>


마침내! 식물을 모니터링 할 장치를 만들었습니다! 자, 해봅시다!

![](https://i.imgur.com/nD0PGDe.png)  

이 코드를 마이크로 비트로 다운로드하십시오. 녹색 식물을 찾고 수분 센서 패널을 토양에 꽂고 감시하십시오. 충분한 물이 없을 때, 부저는 "당신의 식물에 물을 줄 시간입니다!"라고 알려주기 위해 경고합니다. 그리고 식물이 충분한 물을 가지고있을 때, OLED 패널은 당신에게 물이 충분하다는 것과 식물에게 물을 줄 필요가 없음을 보여줄 것입니다.
아주 유용하겠죠?
