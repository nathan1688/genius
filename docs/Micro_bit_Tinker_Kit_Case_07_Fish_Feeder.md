> 손으로 물고기를 먹이는 것에 지쳤습니까? 여기에 당신을 위한 마이크로 프로젝트가 있습니다!
> 이 과정에서는 ADKeypad를 사용하여 물고기에게 먹이를 주는 서보의 움직임을 제어합니다.


## 단계 0 - 사전 빌드 개요
---

![](https://i.imgur.com/QO4eC0H.png)  

이 프로젝트에서 우리는 물고기 먹이 공급 기계를 만들 예정입니다. 서보의 움직임은 ADKeypad의 두 개의 빨간색 버튼으로 제어되며 OLED는 서보의 상태를 나타내는 메시지를 표시합니다.

## 재료 :
---
- 1 x [BBC 마이크로 : 비트] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 마이크로 USB 케이블 1 개
- 1 x [브레이크 아웃 보드] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 x [ADKeypad] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 x [OLED] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 x 서보
- 전선


목표 :
---
- ADKeypad, OLED 및 서보에 대해 알아보십시오.
- 서보로 무언가를 만드십시오.
- OLED로 무언가를 만들어라.


## 만드는 방법
---
### 1 단계 - 구성 요소

![](https://i.imgur.com/FNUJhZ3.jpg)
![](https://i.imgur.com/BAovMFM.jpg)

마이크로 : 비트를 브레이크 아웃 보드에 삽입하고 마이크로 USB 케이블을 꽂은 다음 위 그림과 같이 OLED를 연결합니다. 세 행 중 하나에 플러그를 꽂을 수 있어야합니다.

ADKeypad를 핀 0에 연결하고 서보를 핀 1에 연결하십시오. 와이어의 색상이 브레이크 아웃 보드의 핀 색상과 일치하는지 확인하십시오.

![](https://i.imgur.com/FHD6oh8.jpg)

### 2 단계 - 사전 코딩

우리는 키트 구성 요소를 사용할 수 있도록 코드 패키지를 추가 할 것입니다. 코드 드로어에서 고급을 클릭하면 더 많은 코드 섹션을 볼 수 있고 패키지 추가를위한 코드 드로어의 하단을 볼 수 있습니다.

![](https://i.imgur.com/TF3bfdq.jpg)

그러면 대화 상자가 열립니다. "팅커 키트"를 검색 한 다음이 패키지를 다운로드하려면 클릭하십시오.

![](https://i.imgur.com/nOIgk5u.png)

참고 : 비 호환성 문제로 인해 일부 패키지가 제거된다는 경고 메시지가 표시되면 프로젝트 파일 메뉴에서 프롬프트를 따르거나 새 프로젝트를 만듭니다.

### 3 단계 - 코딩

![](https://i.imgur.com/qLksxfG.jpg)

코드 드로어 안의 Tinkercademy를 ​​클릭하면 키트의 다양한 구성 요소에 대한 맞춤 블록을 찾을 수 있습니다.

![](https://i.imgur.com/6CUN5SW.jpg)

처음에는 항상 OLED를 초기화해야 합니다. 64 및 128은 각각 OLED의 높이 및 폭을 나타냅니다.

![](https://i.imgur.com/gRJsbmX.jpg)

두 가지 조건 만 있기 때문에 'else-if'문 하나만 있으면됩니다.
ADKeypad의 버튼 A를 누르면 서보가 각도 70으로 바뀌고 OLED에 "음식로드 중"이 표시됩니다.
그렇지 않으면 ADKeypad의 B 버튼을 누르면 서보가 각도 20으로 바뀌고 OLED에 "Fishing the fish"가 표시됩니다.
귀하의 요구 사항에 맞게 서보 각도를 조정할 수 있습니다.

이 코드를 직접 입력하지 않으려면 아래 링크에서 전체 프로그램을 다운로드 할 수 있습니다.

[https://makecode.microbit.org/_Azc57HcdM7r1](https://makecode.microbit.org/_Azc57HcdM7r1)

또는 아래 페이지에서 다운로드 할 수 있습니다.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_Azc57HcdM7r1" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>



### 4 단계 - 성공!

올레! 당신은 물고기 먹이 공급 기계를 만들었습니다!
