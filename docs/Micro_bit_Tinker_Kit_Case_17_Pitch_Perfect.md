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
조건은 기본적으로 프로그램이 명령을시작하기 위한 요구 사항을 의미합니다. 따라서 A 버튼을 누르는 if-else 문으로 충분합니다.

다음으로, 게임을 하는 방법에 대한 다른 설명서를 추가합니다. "You have guess which pitch it is by pressing the correct key"를 출력한 다음 사용자가 설명서를 읽을 수 있도록 약 5000ms(5초)의 시간을 줍니다.

### Step 5:

연주되는 사운드의 음높이를 듣기 위해 옥타브 (예 : C)를 4 비트 (4 초) 동안 재생하고, 옥타브 C를 MicroBit LED와 OLED 디스플레이에 표시합니다.

그 다음, 사용자가 알파벳과 ADKeypad로 올바르게 처리할 수 있도록 시간 제한을 둡니다. 또한 특정 옥타브에 어떤 버튼을 눌러야 하는지를 OLED 디스플레이 표시합니다. 예를 들어, 옥타브 C가 재생되고 있을 때 "Left blue button"를 디스플레이하여 표시할 수 있습니다.

OLED 디스플레이와 show string 블록이 반복되는 이유는 디스플레이를 초기화하지 않으면 새로운 텍스트가 작성이 되지 않기 때문입니다.

![](https://i.imgur.com/8abBXgw.png)

### Step 6:  

이제, 여러분은 여러분의 옥타브 테스트를 만들 수 있습니다. 이를 위해서는 옥타브를 재생해야 하며 "Key#1"이라는 메시지로 동시에 지정할 수 있습니다.

그 다음 사용자가 ADKeypad에서 올바른 버튼을 누르면 포인트가 생기고 그렇지 않은 경우 포인트가 생기지 않습니다. 따라서 변수 점수가 올바른 경우 1로, 그렇지 않은 경우 -1로 설정합니다. 따라서 사용자가 올바른 버튼을 눌렀는지 여부에 대한 if-else문을 수행합니다.

사용자에게 정답 여부를 알려주기 위해 체크 표시와 X표시를 사용합니다.

![](https://i.imgur.com/CqWtEwD.png)
![](https://i.imgur.com/jl3ogKg.png)

### Step 7:  

테스트가 완료되면 최신 점수를 표시하여 게임을 종료 할 수 있습니다. 점수가 표시된 상태로 OLED 디스플레이에 "Your score is :" 를 표시할 수 있습니다.

![](https://i.imgur.com/a4LAQac.png)

이러한 코드를 직접 입력하지 않으려면 아래 링크에서 전체 프로그램을 직접 다운로드할 수 있습니다.

[https://makecode.microbit.org/40622-92227-41289-45624](https://makecode.microbit.org/40622-92227-41289-45624)

또는 아래 페이지에서 다운로드할 수 있습니다.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_hFx5DY8ytKqD" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>
