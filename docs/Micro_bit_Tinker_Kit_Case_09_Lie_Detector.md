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

- Octopus LED 와 토양 수분 센서 알아보기 
- 기본 사용 방법 익히기
- 모이스처 센서를 이용하여 무언가를 만들어 보기  


### Step 1 Components  

우선, 토양 수분 센서를 연결하세요. 색상대로 플러그를 꽂아주셔야 합니다.

![](https://i.imgur.com/0VDR4st.jpg)  

다음으로, Octopus LED를 연결해주세요. 세개의 슬롯 중 하나를 사용하면 됩니다.  

![](https://i.imgur.com/SmP85nH.jpg)  


### Step 2 Pre-Coding  

키트구성 요소를 사용하시려면 코드 패키지를 추가해야합니다. 코드 드로잉의 "고급"을 클릭하면, 더 많은 코드 섹션을 볼 수 있으며, "패키지 추가" 의 코드 를 볼 수 있습니다.

![](https://i.imgur.com/BdLQ8AS.jpg)  

대화상자가 열리면, "패키지 추가" 텍스트 필드에서 '팅커키트' 를 찾습니다.

![](https://i.imgur.com/8gYcTp1.png)  

참고 : 비 호환성 문제로 인하여 일부 패키지가 제거된다는 경고 메시지가 표시되면, 프로젝트 파일 메뉴에서 프롬프트를 따르거나 새 프로젝트를 만듭니다.


### Step 3 Coding  

우선, 그림과 같이 OLED 섹션의 블록을 사용하여 OLED를 초기화 합니다.

![](https://i.imgur.com/L68fSV7.jpg)  

이 코드는 토양 수분 센서가 약 1분동안 두 손가락 사이의 전기 전도도를 측정하고 기록하는 것을 허용하는 것 입니다. 그 다음 평균을 계산하는데, 이는 사용자가 거짓을 말하지 않았을 때의 "평온한 상태" 값 입니다.

![](https://i.imgur.com/EdWwt5m.jpg)  

이 코드는 처음 1분동안 얻은 판독 값의 표준 편차를 계산 합니다. 표준 편차는 판독 값이 얼마나 다른지 나타냅니다. 표준 편차가 클수록 판독 값의 편차도 커집니다. "Math.sqrt" 블록스퀘어는 주어진 값을 정의내리고, Javascript로 추가 합니다.

![](https://i.imgur.com/QHI8jfg.jpg)  

초기에 판독 값을 작성하고 기록한 후, 습도 센서는 평균 전기 전도도를 5초 이상 측정 합니다. 표준 편차에 더한 평균 보다 높으면, 사용자가 비정상 적으로 높은 전기전도도를 가지고 있다는 의미 이므로, "거짓" 임을 알 수 있습니다. 그런 다음 LED 화면에 "X"를 표시 합니다.

![](https://i.imgur.com/y5qv2l9.jpg)  

To relieve your tired fingers, you can download the code below.  

[https://makecode.microbit.org/_fadAyyh27Eo3](https://makecode.microbit.org/_fadAyyh27Eo3)  

Or you can download from the page below.  

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_fadAyyh27Eo3" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  


### Step 4 Using It  

우선, 토양 수분 센서의 각 센서부를 손가락 중 하나에 부착해야합니다. 개인적으로 고무 밴드를 사용하는 것이 간단하고 효과적인 것 같습니다. 악어 클립이나 테이프 사용과 같은 다른 방법으로 실험 가능합니다.

![](https://i.imgur.com/QBy1bWj.jpg)  

이제 장치를 켜세요. 이 장치는 피부의 전기 전도도를 기록하고, 평균값과 표준 편차를 표시 합니다.

![](https://i.imgur.com/A5egJ7d.jpg)  

처음 값이 나온 후에, 다시 한 번 확인해보세요! 그 사람이 거짓말을 했다면, 그는 긴장을 했을 것이고, 그 값이 마이크로비트에 표시 될 것 입니다!

![](https://i.imgur.com/Uuq4P62.jpg)  


### Step 5 Success!  

이제 여러분은 마이크로비트로 쉽게 거짓말탐지를 할 수 있습니다!


