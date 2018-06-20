

## Step 0: Pre-build Overview    

![](https://i.imgur.com/mNlJj4l.png)  

이번 프로젝트는 도둑이 들었을 때를 대비해 도둑이 뭔가를 훔쳤을 때 그 사실을 사용자에게 알려주는 간단한 경보 장치를 만들어 보겠습니다.
붉은색 LED는 충돌 센서가 물체에 움직임이 있었음을 감지하면 깜빡입니다. 만약 그렇지 않다면 초록색 LED가 계속 켜져 있을것입니다.
OLED는 현재 장치의 상태를 표시합니다.

## Materials:    
---   

1 x [BBC 마이크로비트](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)    
1 x 마이크로 USB 케이블    
1 x [센서비트](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)    
1 x [LED 모듈](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)    
1 x [충돌 센서](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)     
1 x [OLED](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)    
1 x LED    
2 x Female-Female 점퍼 케이블    


## Goals:    
---  

- LED모듈, 일반 LED, 충돌센서, OLED가 무엇인지 알아보기.  
- 다른 종류의 LED를 이용해서 제작하기.  
- 충돌 센서와 OLED를 사용하여 제작하기.  


## How to Make    
---  

### Step 1 – Components    

![](https://i.imgur.com/208tSHD.jpg)  

LED 모듈을 pin 1에 연결해 주세요.  

![](https://i.imgur.com/wGQpzcn.jpg)  
![](https://i.imgur.com/9yVjSuC.jpg)  

위의 그림과 같이 USB 케이블을 마이크로비트 센서비트 보드에 연결합니다. 케이블의 색상이 센서비트 보드의 핀 색상과 같은지 확인하고 충돌 센서를 Pin 0에 연결한후 LED모듈을 Pin 8에 연결해주세요.  

![](https://i.imgur.com/LQkLriL.jpg)  

### Step 2 – Pre-coding    
We’ll need to add a package of code to be able to use our kit components. Click on Advanced in the Code drawer to see more code sections and look at the bottom of the Code Drawer for Add Package.  

![](https://i.imgur.com/W9LqWIQ.jpg)  

This will open up a dialog box. Search for "tinker kit" and then click it to download this package.  

![](https://i.imgur.com/JjXJhoP.png)  

Note: If you get a warning telling you some packages will be removed because of incompatibility issues, either follow the prompts or create a new project in the Projects file menu.  

### Step 3 – Coding    

![](https://i.imgur.com/yVtxeb2.jpg)  

After that, use blocks under the Tinkercademy section to initialize the OLED and Crash Sensor as shown in the picture.  

![](https://i.imgur.com/z6Gzehg.jpg)  

This part of the code allows the red LED to blink continuously. You can adjust the speed of blinking by changing the pause period.  

![](https://i.imgur.com/6avB2r8.jpg)  

Since there are only two conditions, we need only one ‘else-if’ statement. When the Crash Sensor is pressed, the green Octopus LED will light up. Or else, if no force is applied to the Crash Sensor, the red LED will blink continuously.  

If you don't want to type these code by yourself, you can directly download the whole program from the link below:  

[https://makecode.microbit.org/_LvC6e0UfWH7c](https://makecode.microbit.org/_LvC6e0UfWH7c)  

Or, you can download from the page below:  

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_LvC6e0UfWH7c" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Step 4 – Succeed!    

Let’s download code into it and run it. Let’s find a book or something else and place it on the top of device, then see what will happen. We can see the green light illuminates as showed in the picture below. When we take away the book or something else you placed, you can see the red light starts to flash while the green light turned off.  

![](https://i.imgur.com/wpyHSOF.jpg)   
