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

패키지 추가를 누르면 대화 상자가 열립니다. oled-ssd1306을 검색하여 추가해줍니다.

![](https://i.imgur.com/hykIyTd.png)

Note: If you get a warning telling you some packages will be removed because of incompatibility issues, either follow the prompts or create a new project in the  Projects file menu.

### Step 3:  

![](https://i.imgur.com/ZGzxDCO.png)

First, you have to initialise the OLED screen to a height of 64 and width of 128 so to run the screen in the proper sizing.

Next, you have to set a variable starting score to 0 for the initial play. This means you have a score of 0 at the start of your game. Then you need the OLED display show a text of “Pitch Perfect”.

You need to write a simple instruction on how to start. Thus, a simple sentence “Press A to start ” will do.

### Step 4:  

![](https://i.imgur.com/WmBJnOV.png)

Since at step 3 we wrote that you need to press A to start, we need to write a condition for it. A condition basically means a requirement for a program to start loading its instructions. Thus, an if-else statement of the A button being pressed would suffice. Moreover, this will be nested on a forever bracket.

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
