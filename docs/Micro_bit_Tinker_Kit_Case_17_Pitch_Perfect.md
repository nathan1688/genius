![](https://i.imgur.com/HYkxR5d.jpg)


## 목표 
---

•	ADKeypad, OLED, buzzer를 사용하는 방법.
•	ADKeypad, OLED, buzzer를 이용해 프로젝트 제작.
•	if-else 문법 익히기.

![](https://i.imgur.com/lNJbWPG.jpg)
 
 
## Materials Needed  
---

- 1 x [BBC 마이크로비트 보드](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)  
- 1 x 마이크로 USB 케이블
- 1 x [부저 모듈](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)  
- 2 x [F-F 점퍼선](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)  
- 1 x [OLED](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)  
- 1 x [ADKeypad](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)  
- 1 x [지니어스 키트 센서비트 보드](http://www.icbanq.com/shop/templete_list.asp?t_idx=163) 


## 프로젝트 만드는 방법  
---

### Step 1:  

먼저, 부저를 핀 0에 꽂고 양극(대개 더 긴 쪽)이 노란 색 신호 핀에 연결되고 음극 끝이 지니어스 키트 센서 비트의 검은 색 접지 핀에 연결합니다.

ADKeypad를 핀 1에 연결하여 와이어의 색상과 지니어스 키트 센서비트 보드의 색이 일치하는지 확인합니다. 그런 다음, 지니어스 키트 센서비트 보드의 하단 좌측 소켓에 OLED화면을 부착합니다.

### Step 2:

![](https://i.imgur.com/CmT2k2T.png)

키트 구성 요소를 사용하려면 코드 편집기에 패키지를 추가해야 합니다. 고급을 클릭하면 패키지 추가라는 섹션이 표시됩니다.

패키지 추가를 누르면 대화 상자가 열리고 oled-ssd1306을 검색하여 추가해줍니다.

![](https://i.imgur.com/hykIyTd.png)

참고:비호환성 문제로 인해 일부 패키지가 제거된다는 경고가 표시되면 프로젝트 파일 메뉴에서 안내 메시지를 따르거나 새 프로젝트를 만드세요.

### Step 3:  

![](https://i.imgur.com/ZGzxDCO.png)

먼저, 화면을 적절한 크기로 작동하기 위해서는 64의 높이와 128의 너비로 OLED화면을 초기화해야 합니다.

다음으로 시작 점수를 0으로 설정해야 합니다. 이것은 게임 시작 시 0점으로 시작함을 의미합니다. 그리고 OLED 디스플레이에 "Pitch Perfect "라는 텍스트를 출력합니다.

"Press A to start"라는 문장으로 시작하는 방법에 대해 설명을 합니다.
### Step 4:  

![](https://i.imgur.com/WmBJnOV.png)

step 3에서 A를 눌러야 시작할 수 있다는 내용을 작성했으므로 조건문을 추가로 작성해보겠습니다.
조건은 기본적으로 프로그램이 명령을시작하기 위한 요구 사항을 의미합니다. 따라서 A 버튼을 누르는 if-else 문으로 충분합니다. 또한, 이것은 괄호 안에 중첩됩니다.

Next, you have to write another set of instructions on how to play the game. What I wrote was : “You have guess which pitch it is by pressing the correct key”. Then you have to have a timeout around 5000ms (5 seconds) to let the user read the instructions.

### Step 5:

You are gonna introduce the user to listen to the pitch of the sound being played. What I did was to play the pitch (for example: C) for 4 beat (4 seconds), flash the led on the MicroBit of the pitch C and OLED display on the screen itself.

After that, I will put in a timeout so the user can process the pitch to the correct alphabet and the ADKeyboard. Additionally, you can put in the OLED screen on what buttons are to be pressed for a certain pitch. Example, when Pitch C is being played, I wrote “Left blue button” to indicate that is the button.

If you are wondering, why the intialise OLED display and show string block is repeated, it is because it would simulate a refresh in web browser. If you do not initalise the display, the text would just be brought down instead of new text being created.

![](https://i.imgur.com/8abBXgw.png)

### Step 6:  

Once the user have gone through the mini-briefing of how the pitch sounds, you can get them ready. You can have a countdown for them to get ready on the game itself.

Now, you can build your pitch tests. So, to do that, you need to play a pitch and you can customise by displaying by any image on the MicroBit and a message “Key #1” at the same time.

Then, if the user pressed the correct button on the ADKeypad, they would get a point. If not, no points. Thus you set the variable score to change by 1 if the get it correct and otherwise, a -1. Thus, an if-else statement on whether the user pressed the correct button will do.

To let the user know if they got the correct answer, you can display of an image tick for a correct answer and a cross for a wrong answer.

Repeat this step so you can have many tests to play with!

![](https://i.imgur.com/CqWtEwD.png)
![](https://i.imgur.com/jl3ogKg.png)

### Step 7:  

Once you are contempted with your tests, you can end the game by showing the latest scores. You can display in the OLED screen “Your score is:” with the variable score shown. Put a smiley for fun sake.
And you are done! Enjoy the game.

![](https://i.imgur.com/a4LAQac.png)

If you don't want to type these code by yourself, you can directly download the whole program from the link below.

[https://makecode.microbit.org/40622-92227-41289-45624](https://makecode.microbit.org/40622-92227-41289-45624)

Or you can download from the page below.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_hFx5DY8ytKqD" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>
