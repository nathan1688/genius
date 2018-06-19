

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


## How to Make  
---

#### Step 1  

After connecting one end of the USB cable to your computer, connect the other end to the micro:bit as shown in the picture below.Then connect the side of the micro:bit where the pins are located to the breakout board.  

![](https://i.imgur.com/DdX7fE9.jpg)  

#### Step 2  

Plug in the buzzer Brick to Pin 0.  
Plug in the ADKeypad to Pin 2.  
Make sure the colour of the wire of the buzzer and the ADKeypad follows the colour of the pins on the breakout board.  
 
![](https://i.imgur.com/EhTHEaU.jpg)  
 
#### Step 3  

Click on Advanced in the Code Drawer to see more code sections.  

![](https://i.imgur.com/8wKkVPE.jpg)  

To code for our extra kit components (the ADKeypad and the buzzer), we have to add a package of code.Look at the bottom of the Code Drawer for “Add Package” and click it. This will open up a dialogue box.  
Search for "tinker kit" and click on it to download this package.  

![](https://i.imgur.com/gvuN2rQ.png)  

Note: If you get a warning telling you some packages will be removed because of incompatibility issues, either follow the prompts or create a new project in the Projects file menu.  


#### Step 4  

Next, let’s create a conditional statement as shown in the picture. This ‘if-then’ block of code is under the code section “Logic” of the code drawer.The code shown below means that when button A is pressed on the ADKeypad while the ADKeypad is plugged in at pin P2 of the breakout board, the buzzer will play a sound of 175 hertz.  

![](https://i.imgur.com/5bFh8GO.jpg)  
 
Since there are 5 buttons, we need to code 5 similar conditional statements. Each button controls a sound of a particular pitch. So press each buttion, we will get sounds of different pitches.  

![](https://i.imgur.com/mAvF9Oi.jpg)  

If you don't want to type these code by yourself, you can download it directly from the link below:  

[https://makecode.microbit.org/_Aw1LAP8VdCs0](https://makecode.microbit.org/_Aw1LAP8VdCs0)

Or, you can download from the page below:  

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_Aw1LAP8VdCs0" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>    


Success! Now you have your own Micro:bit Music Machine.    
