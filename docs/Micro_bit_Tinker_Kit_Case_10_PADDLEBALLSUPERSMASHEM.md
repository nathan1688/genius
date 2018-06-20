
![](https://i.imgur.com/ngNx9A3.jpg)  

JavaScript를 사용하여 5x5 디스플레이에서 간단하지만 재미있는 게임을 만들 수 있습니다!
(PADDLEBALLSUPERSMASHEM은 다른 그래픽 게임과 유사할 수 있습니다!!)


## Step 0 – Pre Build Overview    
---  

이 프로젝트에서는 벽에 공을 튀기는 간단한 게임을 제작합니다. 만약 공을 놓치면, 바로 죽는 게임이죠! 
당신의 도전이 계속 되면, 게임의 난이도는 계속 증가합니다.

## Goals    
---  

- 마이크로비트 마이크로컴퓨터에 대해 더 자세히 알아보세요.
- 간단한 게임을 프로그래밍하는 방법을 배워보세요.


## Material    
---   

- 1 x [마이크로비트](http://www.elecfreaks.com/estore/bbc-micro-bit-board-for-coding-programming.html)  
- 1 x 마이크로 USB 케이블 

![](https://i.imgur.com/Im2BXNd.jpg)  


## How to Make    
--  

### Step 1: Components     

우선, 마이크로비트를 컴퓨터와 연결하세요. 다른 구성 요소는 필요하지 않습니다.

![](https://i.imgur.com/fqrpqTW.jpg)  


### Step 2： Pre-coding    

우리는 키트 구성 요소를 사용할 수 있도록 코드 패키지를 추가 할 것 입니다. 코드 드로어에서 "고급"을 클릭하면, 더 많은 코드 섹션을 볼 수 있으며, "패키지 추가"에 대한 내용을 볼 수 있습니다.

![](https://i.imgur.com/I2L5019.jpg)  

그러면 대화 상자가 열립니다. "팅커 키트"를 검색한 다음 패키지를 클릭하여 패키지를 다운로드 하세요.

![](https://i.imgur.com/8a7kDKF.png)  

참고: 비 호환성 문제로 인하여 일부 패키지가 제거 될 것 이라는 경고 메시지가 표시되면, 프로젝트 파일 메뉴에서 프롬프트를 따르거나 새 프로젝트를 만들어야합니다.


### Step 3: Coding    

![](https://i.imgur.com/SfkOKmO.png)  

우선, 변수를 정의하세요 ! 우리는 공의 위치, 속도와 방향, 패들의 길이와 위치, 마지막으로 점수를 저장하기 위하여 많은 변수들이 필요합니다.

![](https://i.imgur.com/oYBRGY9.png)  

다음으로, 우리는 패들을 제어하는 기능들을 프로그램 할 것 입니다.
xb는 왼쪽에서부터 패들의 첫번째 픽셀의 위치를 나타내며, yb는 패들의 길이를 나타냅니다. 왼쪽과 오른쪽 기능은 xb를 제어하고 패들을 이동시키고 보드 기능은 패들을 화면에 표시합니다.

![](https://i.imgur.com/lQ0drJR.png)  

다음으로, 볼이 움직일 때를 제어하는 함수를 포함합니다. 처음에는 공이 1초마다 움직이지만, 당신이 전진할 때 공은 짧은 간격으로 계속 움직입니다. 매우 흥미진진 하죠!

![](https://i.imgur.com/c6jUmNb.png)  

이제 공이 주변 환경과 어떻게 상호 작용하는지 제어하는 기능을 프로그래밍합니다. 공이 측면을 치면 수평 운동으로 반전 되지만, 수직 운동은 동일하게 유지 됩니다. 공이 천장에 부딪힐 때 어떤 방향으로든 튀어나와 게임을 더 재미있게 만들 수 있습니다.

![](https://i.imgur.com/MrcNyKJ.png)  

가장 중요한 것은, 공이 패들에 닿는 지 확인해야합니다. 놓친 다면 점수를 잃게 됩니다. 놓지지 않을 경우 공이 임의의 방향으로 튀어나와서 게임의 난이도가 높아집니다.

![](https://i.imgur.com/WIXWKV0.png)  

마지막으로 볼을 움직이기 위해 시계 역할을 하는 for 루프가 있습니다. 또한, 우리는 외륜을 움직이는 onButtonPressed() 함수를 가지고 있습니다. 또한, 우리는 패들을 움직이는 onButtonPressed() 함수를 가지고 있습니다.
아래 링크에서 코드를 바로 받아서 사용하세요.

[https://makecode.microbit.org/63331-03858-42547-81536](https://makecode.microbit.org/63331-03858-42547-81536)  

아니면,이 페이지에서 다운로드 가능합니다.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:63331-03858-42547-81536" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Step 4: Using It    

![](https://i.imgur.com/yARLugY.jpg)  

마이크로 컨트롤러를 컴퓨터에 연결하고 프로그램을 실행하세요!

![](https://i.imgur.com/cV3q2Ar.jpg)  

12점 이상을 획득하면, 승리를 할 수 있습니다!


### Step 5: Success!    

이제 PADDLEBALLSUPERSMASHEM을 5x5 디스플레이에 프로그래밍 했습니다 !
