당신에게 몰래 놀래키려는 사람들이 싫나요? 여기에 맞는 마이크로가 있습니다 : 당신을위한 비트 프로젝트! 이 코스에서는 모션 센서, 습도 센서 및 코딩 방법을 배우게됩니다.

목표 :
---
- PIR 센서 브릭 및 습기 센서에 대해 알아보십시오.
- PIR 센서 브릭으로 무언가를 만드십시오.
- 수분 센서로 무언가를 만드십시오.

## 재료 :
---

- 1 x [BBC 마이크로 : 비트] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 마이크로 USB 케이블 1 개
- 1 x [브레이크 아웃 보드] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 X [미니 버저] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 X [Octopus PIR 센서 브릭] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 X [수분 센서] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 2 X 암 - 암 점퍼 와이어


## 만드는 방법
---
### 1 단계
USB 케이블의 한쪽 끝을 컴퓨터에 연결 한 후 다른 쪽 끝을 그림과 같이 마이크로 비트에 연결하십시오. 핀이있는 곳의 마이크로 비트를 브레이크 아웃 보드에 연결하십시오.

![](https://i.imgur.com/64lAG8S.jpg)

### 2 단계

부저를 핀 0 (브레이크 아웃 보드의 번호 '0'옆에있는 핀)에 연결하십시오. 습기 센서를 핀 3에 연결하십시오. 모션 센서를 핀 1에 연결하십시오. 부저와 ADKeyboard의 와이어 색상이 브레이크 아웃 보드의 핀 색상을 따르도록하십시오.


![](https://i.imgur.com/NuBmxhy.jpg)  
![](https://i.imgur.com/Rj1DnJb.jpg)  
![](https://i.imgur.com/pHfDOO8.jpg)  


### 3 단계
더 많은 코드 섹션을 보려면 코드 드로어에서 "고급"을 클릭하십시오.
추가 키트 구성 요소 (ADKeyboard 및 부저)를 코딩하려면 코드 패키지를 추가해야합니다.

![](https://i.imgur.com/Lb5u8N0.jpg)  

"Add Package"에 대한 코드 드로어 하단을보고 클릭하여 대화 상자를 엽니 다. "팅커 키트"를 검색 한 다음 패키지를 클릭하여 패키지를 다운로드하십시오.

![](https://i.imgur.com/pBgBfAm.png)  

참고 : 비 호환성 문제로 인해 일부 패키지가 제거된다는 경고 메시지가 표시되면 프로젝트 파일 메뉴에서 프롬프트를 따르거나 새 프로젝트를 만듭니다.

![](https://i.imgur.com/SRt0dDo.png)  

코드 드로어 안의 Tinkercademy를 ​​클릭하면 키트의 다양한 구성 요소에 대한 맞춤 블록을 찾을 수 있습니다.

![](https://i.imgur.com/WC0lzLU.png)  

이 프로젝트에서는 습도 센서와 모션 센서의 블록 판독 값을 사용하려고합니다.   

### 4 단계
이 단계에서는 블록 편집기를 사용하여 Micro : bit를 코딩합니다. 먼저 "On Start"블록 아래에 "Show Icon"블록을 오른쪽 그림과 같이 배치하여 시작 화면을 코딩합니다.
그러면 마이크로 비트가 켜질 때마다 아이콘이 화면에 나타납니다.

![](https://i.imgur.com/NFbqCkL.png)  

### 5 단계
다음으로 습도 센서 값을 사용하여 음악을 만들어 봅시다.
"Music"코드 섹션에서 "Play Tone"블록을 선택하고 수분 센서 코드 블록의 값을 그 안에 넣으십시오.
피치는 왼쪽 이미지와 같이 센서 값에 다른 숫자를 곱하여 조정할 수 있습니다.

![](https://i.imgur.com/DfFWFin.png)  

### 6 단계
마지막으로 모션 센서가 움직임을 감지 할 때 부저 소리를냅니다. 마이크로 비트는 움직임이없는 경우에만 화면에 아이콘을 표시합니다.
이는 조건부 (if-then-else) 문을 사용하고 오른쪽 그림과 같이 해당 스폿에 관련 블록을 삽입하여 수행 할 수 있습니다.

![](https://i.imgur.com/fbTZLgN.png)  

이 코드를 직접 입력하지 않으려면 아래 링크에서 전체 코드를 직접 다운로드 할 수 있습니다.

[https://makecode.microbit.org/_8xYPibiLdeYR](https://makecode.microbit.org/_8xYPibiLdeYR)  

또는 아래 페이지에서 다운로드 할 수 있습니다.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_8xYPibiLdeYR" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>    


이제 다음 코드를 마이크로 비트로 저장하고 사용해보십시오!
성공! 당신은 지금 당신 자신의 마이크로 : 비트 모션 디텍터를 가지고 있습니다!
