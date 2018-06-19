

![](https://i.imgur.com/cqLH6Bs.jpg)  

## 목표  
---

•	ADKeypad를 사용하는 방법.  
•	ADKeypad를 이용해 프로젝트 제작.  
•	Buzzer를 이용한 프로젝트 .  


## 구성품목  
---

1 x [BBC 마이크로비트 보드](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)  
1 x 마이크로 USB 케이블  
1 x [지니어스 키트 센서비트보드](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)  
1 x [부저 모듈](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)  
1 x [ADKeypad](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)  

![](https://i.imgur.com/BJ5WTuI.jpg)  

Tips: 위의 모든 구성요소를 활용 하고 싶으시다면 해당 키트를 구매해 주세요 [마이크로비트 지니어스 키트](http://www.icbanq.com/shop/templete_list.asp?t_idx=163).  


## 프로젝트 만드는 방법  
---

#### Step 1  

USB 케이블을 컴퓨터에 연결 한 후 아래 그림과 같이 다른 쪽 끝을 마이크로비트에 연결합니다. 그런다음 핀이 있는 마이크로비트를 센서비트에 연결합니다.  

![](https://i.imgur.com/DdX7fE9.jpg)  

#### Step 2  

부저 모듈을 Pin 0 에 연결해 주세요.  
ADKeypad 모듈을 Pin 2 에 연결해 주세요.  
부저 모듈과 ADKeypad 모듈의 케이블 색상이 센서비트의 핀 색상과 동일한 곳에 결합 하였는지 확인해 주세요.
 
![](https://i.imgur.com/EhTHEaU.jpg)  
 
#### Step 3  

마이크로비트 블럭 에디터에서 Advanced 를 클릭해 본다면 좀더 많은 블럭코드를 사용 할 수 있습니다.  

![](https://i.imgur.com/8wKkVPE.jpg)  

추가 키트 구성 요소를 코딩하려면 코드 패키지를 추가 해야합니다. "Add Package"의 하단을 클릭하면 대화 상자가 열리고 "tinker kit"를 검색하여 패키지를 다운로드 해 주세요.  

![](https://i.imgur.com/gvuN2rQ.png)  

Note: 만약 비 호환성 문제로 인해 일부 패키지가 제거된다는 경고 메시지가 표시된다면 프로젝트 파일 메뉴에서 프롬프트를 새로 만들면됩니다.  


#### Step 4  

아래 그림과 같이 조건문을 만들어 보겠습니다. 'if-then' 코드 블록은 코드 카테고리에서 "Logic"코드 섹션 아래에 있습니다.
아래에 표시된 코드는 ADKeypad가 센서비트 보드의 P2 핀에 연결 되어있는 동안 ADKeypad에서 A 버튼을 누르면, 부저는 175Hz 주파수의 소리를 재생합니다.

![](https://i.imgur.com/5bFh8GO.jpg)  
 
ADkeypad에는 5개의 버튼이 있음으로, 5개의 유사한 조건문을 코딩해야합니다.
각 버튼은 특정 음의 사운드를 제어합니다. 따라서 각각의 버튼을 누르면 다른 음의 소리가 나옵니다.

![](https://i.imgur.com/mAvF9Oi.jpg)  

이 코드를 직접 만들기가 어렵다면 아래의 링크를 통해 직접 다운로드가 가능합니다.:  

[https://makecode.microbit.org/_Aw1LAP8VdCs0](https://makecode.microbit.org/_Aw1LAP8VdCs0)

혹은, 아래의 페이지에서 다운로드 할 수 있습니다.:  

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_Aw1LAP8VdCs0" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>    


자!!이제 자신 만의 마이크로비트 뮤직 키트가 생겼습니다!    
