![](https://i.imgur.com/2Pcz8rt.jpg)

마이크로비트를 이용하여, 거짓말 탐지기를 만들어보자! 
모이스처 센서 하나면, 진실만을 말하게 된다!


## Step 0 – Pre Build Overview    
---

이 프로젝트에서 우리는, 피부의 전기 전도도를 측정하여 작동하는 간단한 거짓말 탐지기를 만들어 볼 것 입니다.
사람은 긴장을 하면 피부의 전기 전도도가 증가하게 되는데, 모이스처 센서가 이를 감지할 수 있습니다.
이러한 원리로 어떤사람이 진실을 말하고 있는지를 판단할 수 있게 해줍니다.


## Materials     
---  

- 1 x [마이크로비트](http://www.elecfreaks.com/estore/bbc-micro-bit-board-for-coding-programming.html)  
- 1 x 마이크로 USB 케이블 
- 1 x [브레이크 아웃 보드](http://www.elecfreaks.com/estore/elecfreaks-micro-bit-breakout-board.html)  
- 1 x Octopus OLED  
- 1 x [모이스처 센서](http://www.elecfreaks.com/estore/octopus-soil-moisture-sensor-brick.html)  

팁: 위의 모든 구성 요소를 원하신다면, [마이크로비트 Genius KIT](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)가 필요할 수 있습니다.

![](https://i.imgur.com/eDFUaml.jpg)  


## Goals    
---  

- Get to know the Octopus LED and Soil Moisture Sensor   
- Learn basic statistics   
- Make something using the moisture sensor   


### Step 1 Components  

First of all, plug in the soil moisture sensor. Match the colors and note down what pin you plug for it will influence later procedures. 

![](https://i.imgur.com/0VDR4st.jpg)  

Next, plug in the Octopus LED. Any of the three slots should do.   

![](https://i.imgur.com/SmP85nH.jpg)  


### Step 2 Pre-Coding  

We’ll need to add a package of code to be able to use our kit components. Click on “Advanced” in the Code drawer to see more code sections and look at the bottom of the Code Drawer for “Add Package”.  

![](https://i.imgur.com/BdLQ8AS.jpg)  

This will open a dialog box. In “Add Package” text field search tinker kit.   

![](https://i.imgur.com/8gYcTp1.png)  

Note: If you get a warning telling you some packages will be removed because of incompatibility issues, either follow the prompts or create a new project in the Projects file menu.  


### Step 3 Coding  

First of all, initialize the OLED using blocks in the OLED section as shown in the picture.  

![](https://i.imgur.com/L68fSV7.jpg)  

This part of the code allows the soil moisture sensor to measure and record down the electrical conductivity between the two fingers every few seconds for about a minute. Then, it calculates the average. This is the “calm” value when the user has not told any lies.  

![](https://i.imgur.com/EdWwt5m.jpg)  

This part of the code calculates the standard deviation of the readings obtained in that first minute. The standard deviation indicates how different the readings were. A larger standard deviation means more variance in the readings. The “Math.sqrt” block square roots the given value and was added in Javascript.  

![](https://i.imgur.com/QHI8jfg.jpg)  

After the initial readings have been made and recorded, the moisture sensor now measures the average electrical conductivity over five seconds. If it is higher than the average added to the standard deviation, we can conclude that the user has an abnormally high electrical conductivity and is thus lying. Then, the LED screen would show an “X”shape.  

![](https://i.imgur.com/y5qv2l9.jpg)  

To relieve your tired fingers, you can download the code below.  

[https://makecode.microbit.org/_fadAyyh27Eo3](https://makecode.microbit.org/_fadAyyh27Eo3)  

Or you can download from the page below.  

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_fadAyyh27Eo3" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Step 4 Using It  

First of all, you will have to attach each prong of the soil moisture sensor to one of your fingers. Personally, I found that using rubber bands was a simple and effective way to do so. You can experiment with different methods, such as using crocodile clips or tape. 

![](https://i.imgur.com/QBy1bWj.jpg)  

Now, turn on the device. The device will record the electrical conductivity of your skin under calm circumstances. Then, it will give the average value and its standard deviation.   

![](https://i.imgur.com/A5egJ7d.jpg)  

After the initial readings have been made, ask again! If the person has lied, he will become nervous and the device can pick up on that, resulting in a cross being displayed.   

![](https://i.imgur.com/Uuq4P62.jpg)  


### Step 5 Success!  

Voila! Now you can test lies with this machine easily.  


