micro_bit_Tinker_Kit_Case_12_Remote_Control_Everything.md

![](https://i.imgur.com/utimqzn.jpg)  

리모콘 처럼 제어하려는 마이크로 비트 프로젝트를 구상하고 있습니까?
친구와 함께 2개를 사거나 스페어 마이크로 : 비트를 포함해서 2 마이크로 비트의 원격 제어 프로젝트를 만듭니다. (단! 친구의 마이크로비트를 뺏지 마세요!)


## 목표
---
  
- 이 메뉴얼에서 micro : bit 자동차에 대한 원격 제어를 활성화합니다.
- 예비 마이크로 : 비트를 사용하여 기존 프로젝트에 대한 원격 제어를 만드십시오!
- 모든 것을 Remote Control!


## 재료
---
 
- 1 x [BBC 마이크로 : 비트] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 마이크로 USB 케이블 1 개
- 1 x 배터리 상자
- AA 배터리 2 개
- 1 x [마이크로 : bit car] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
또는
- 원격 제어하려는 프로젝트 1 개


## 만드는 방법
---

### 1 단계

라디오 그룹을 makecode로 설정하십시오. 이렇게하면 송신기와 수신기가 동일한 채널에 있는지 확인할 수 있습니다.
리모컨의 각 버튼 사용법을 생각해보십시오.
라디오는 표시된 블록을 사용하여 각 버튼 누름 이벤트 블록마다 다른 번호를 보냅니다.
라디오 보관함 아래에서 이러한 블록을 찾을 수 있습니다.
이것을 마이크로 컨트롤러에 다운로드하면 리모컨으로 사용할 수 있습니다.
이제 마이크로 : 비트 리모컨의 각 버튼이 다른 명령을 보냅니다!

![](https://i.imgur.com/7FMhilE.png)    


### 2 단계

마이크로 : 비트 자동차 프로젝트 (또는 원격 제어하려는 특정 프로젝트)에서 동일한 라디오 그룹 블록을 시작 블록에 추가하십시오.
 
이렇게하면 원격 제어하려는 프로젝트가 올바른 명령을 듣게됩니다!

![](https://i.imgur.com/2yEuF4F.png)    


### 3 단계

버튼을 누를 때마다 리모콘에서 보낸 숫자를 기억하십니까? 우리는 그것을 사용하여 행동을 촉발시킵니다.
라디오 받침대에 표시된대로 라디오 수신 블록을 찾습니다.
if-then 블록을 사용하여받은 번호가 버튼 A를 누를 때 보낸 번호인지 확인하십시오.
마이크로 : 비트 자동차가 왼쪽으로 바뀌는 코드를 가져 와서이 if-then 블록 안에 넣으십시오.
우리는 또한 일어날 예정이었던 것을 보여주기 위해 왼쪽을 가리키는 주도 표시를 추가했습니다.
핀을 0에 디지털로 기록한 후 왼쪽 서보를 끕니다.


![](https://i.imgur.com/c8EQV91.png)    


### 4 단계

당신의 마이크로 : 비트 자동차를 오른쪽으로 바꾸는 코드에 똑같이 하십시오!
나중에 오른쪽 바퀴를 끄십시오.
각 명령을받은 후에는 항상 바퀴를 멈추지 않고 선택할 수 있습니다. 그러나 자동차가 계속 원형을 그리는 상황에 직면하게됩니다.
이 프로그램을 마이크로 : 비트 자동차에 다운로드하십시오.

![](https://i.imgur.com/Z0xJGlt.png)    

이 코드를 직접 입력하지 않으려면 아래 링크에서 전체 프로그램을 다운로드 할 수 있습니다. 

**Remote Control:** [https://makecode.microbit.org/_gH73AW4Dy1rP](https://makecode.microbit.org/_gH73AW4Dy1rP)  
**Receiver:** [https://makecode.microbit.org/_4am87cCWb0e9](https://makecode.microbit.org/_4am87cCWb0e9)  

또는 아래 페이지에서 다운로드 할 수 있습니다.

**리모콘:**

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_TKE3rA7CqL2w" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>    


**리시버:**    

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_4am87cCWb0e9" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>    


### 신난다!
  
이제 모든 코드가 마이크로비트에 잘 어울립니다. 배터리 팩을 연결하고 이동하십시오! 주변에서 놀고 A + B 버튼으로 보낼 수있는 다른 명령을 보거나 버튼 대신 다른 종류의 입력을 시도하십시오. 그런 다음 모든 다른 micro : bit 프로젝트를 원격 제어하십시오. 자리에 앉은 채로 세계를 지배하세요!
