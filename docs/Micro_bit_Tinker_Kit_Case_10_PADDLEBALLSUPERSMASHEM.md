
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

We now program the functions that control how the ball interacts with its surroundings. When the ball hits the side, its horizontal movement is reversed but its vertical movement remains the same. When the ball hits the ceiling, it can rebound in any direction, to make the game more fun.   

![](https://i.imgur.com/MrcNyKJ.png)  

Most importantly, we need to see if the ball hits the paddle. If it misses, you lose, displaying your score! If it doesnt miss, the ball will also rebound in a random direction, and the difficulty of the game will increase.  

![](https://i.imgur.com/WIXWKV0.png)  

Lastly, we have a for loop which acts as a clock so that the ball keeps moving. Also, we have the onButtonPressed() functions that move the paddle.   
Save your tired fingers and download the code from the link below.  

[https://makecode.microbit.org/63331-03858-42547-81536](https://makecode.microbit.org/63331-03858-42547-81536)  

Or you can download from this page.  

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:63331-03858-42547-81536" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Step 4: Using It    

![](https://i.imgur.com/yARLugY.jpg)  

Just connect the microcontroller to your computer, and run the program! Easy!  

![](https://i.imgur.com/cV3q2Ar.jpg)  

If you score more than 12 points, you will be rewarded with a smiley face! Otherwise, the program may not be very pleased…  


### Step 5: Success!    

Voila! You have now programmed PADDLEBALLSUPERSMASHEM on a 5 by 5 display. You should be proud of yourself.    
