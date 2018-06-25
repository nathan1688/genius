micro_bit_Tinker_Kit_Case_21_Flappy_Bird.md

![](https://i.imgur.com/EWlMcgc.jpg)


마이크로비트와 파이썬을 사용하여 악명 높은 버전의 플래피 버드 게임으로 비행기를 타고 파이프의 꿈을 이루세요.

Raffles Institution의 Cheryl이 제작했습니다.

![](https://i.imgur.com/H6Kz8Ky.gif)


## 목표
---

우리는 5x5 LED를 통해 게임을 만들 것 입니다. 이 과정에서 배울 내용은 다음과 같습니다.
첫번째 단계는 마이크로비트 라이브러리를 파이썬으로 가져오는 것입니다.
그 다음 화면에서 '준비 완료' 메시지가 나오고 카운트 다운이 시작됩니다.
- 1행: 마이크로비트 프로그램을 가져옵니다.
- 4행: '준비 완료' 메시지가 나옵니다. 큰 따옴표는 문자열을 나타냅니다.
- 5-10행: sleep () 함수를 사용하여 화면의 각 숫자를 1 초 (또는 측정에 관련된 1000 밀리 초) 동안 깜박입니다.
- 11행: 새와 벽을 그리는 화면을 지웁니다.

**참고:**
다른 사람들을 위해 자신의 코드를 설명하기 위해 코멘트를 추가하는 것이 좋습니다. '#'으로 설명을 추가합니다.


## 준비물 
---

- 1 x [BBC 마이크로비트 보드](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 x 마이크로 USB 케이블  


## 왜 파이썬인가?  
---

- 영어 처럼 읽기 - 파이썬은 읽기 쉬운 언어 중 하나입니다. 환상적인 초보자 용 언어입니다.
- 다용도 - Python은 정당한 이유로 업계 표준입니다. 많은 것을 할 수 있습니다. 이것이 Google과 YouTube가 백엔드 소프트웨어의 일부로이 언어를 사용하는 이유입니다.
- 활동적인 커뮤니티 - 파이썬은 초보자에게 가장 인기있는 언어 중 하나입니다. 수많은 리소스가 있으며 코드를 살펴 보는 데 도움이되는 정보가 많습니다. 코드 작성 과정에서 걸림돌이되는 것을 극복하는 데 도움이된다는 것을 알 수 있습니다.



## 파이썬에서 코딩을 시작하려면 어떻게해야합니까?  
---  

[공식 마이크로비트 파이썬 에디터](http://www.python.microbit.org/)로 이동을 하거나 [오프라인 파이썬 편집기](https://codewith.mu/)를 다운로드하여 코드를 작성한 후 마이크로비트로 보내기만 하면 됩니다. 매번 업로드하는 귀찮은 과정을 줄이기 위해 [마이크로비트 시뮬레이터](https://create.withcode.uk/)를 사용할 수도 있습니다.

설정이 완료되면 마이크로 USB 케이블을 사용하여 마이크로비트를 컴퓨터에 연결합니다. 

모든 프로그래밍 문제를 해결하는 방법은 그것을 달성 할 수 있는 바이트 크기로 나누는 것입니다. 우리가 무엇을 필요로하는지 보도록하겠습니다. 게임의 데모를 보려면 비디오를 참조하십시오.
화면이 시작되면 'READY'메시지와 카운트 다운이 표시됩니다.

새를 나타내는 좌표를 작성한다.
버튼 A를 눌러 새를 움직인다.
새가 통과하는 파이프의 수를 추적해라.
새가 지나갈 수 있는 벽을 작성한다.
새가 벽과 충돌하면 게임은 끝난다.
이 단계를 직접 수행해보세요. 필요한 경우 단계를 더 작은 단계로 세분화합니다.

## 만든는 방법 
--- 

### Step 1 – Hello, World!  

![](http://www.elecfreaks.com/estore/download/flappy-bird-2.gif)
![](http://www.elecfreaks.com/estore/download/flappy-bird-3.png)

첫번째 단계는 마이크로비트 라이브러리를 파이썬으로 가져오는 것입니다.
그 다음 화면에서 '준비 완료' 메시지가 나오고 카운트 다운이 시작됩니다.
- 1행: 마이크로비트 프로그램을 가져옵니다.
- 4행: '준비 완료' 메시지가 나옵니다. 큰 따옴표는 문자열을 나타냅니다.
- 5-10행: sleep () 함수를 사용하여 화면의 각 숫자를 1 초 (또는 측정에 관련된 1000 밀리 초) 동안 깜박입니다.
- 11행: 새와 벽을 그리는 화면을 지웁니다.

참고: 다른 사람들을 위해 자신의 코드를 설명하기 위해 코멘트를 추가하는 것이 좋습니다. '#'으로 설명을 추가합니다.
파이썬에서는 4행 텍스트의 스크롤 속도를 줄일 수 있습니다.


### Step 2 – Fly, Birdie!  

![](http://www.elecfreaks.com/estore/download/flappy-bird-4.png)
우리는 새의 이미지를 만들어야 합니다. 5X5의 LED를 사용하지만 조금 더 현실적인 움직임을 위해 100개의 위치로 나눌 것입니다. 
이 경우 화면 상단의 위치는 Y0=0이고 버튼은 y=99이므로 100개의 위치가 있습니다. 시작 위치는 y=50입니다.
13행: y=0이 상단이고 y=99가 하단에 있기 때문에 중간에 새의 시작 위치를 설정합니다.
17행: 변수 y에 저장된 값을 20으로 나누어 새 크기를 화면으로 축소합니다.
18행: x, y및 밝기의 3가지 매개 변수를 가진 display.set_pixel함수를 사용하여 화면에 새가 표시됩니다. 
x좌표는 1이므로 두번째 열에 표시됩니다. 
우리는 50을 20으로 나눠서 반올림했기 때문에 현재 y 좌표는 2입니다. 
(참고:인덱스는 일반적으로 컴퓨터 프로그래밍의 경우 0에서 시작되므로 위에서 아래로 행이 0-4이고 왼쪽에서 오른쪽으로 행이 0-4입니다.)
밝기는 0에서 9 사이의 정수가 될 수 있으며 9가 가장 밝습니다. 이 경우 눈이 피로해지기 때문에 7로 설정합니다. 
파이썬은 들여 쓰기를 사용하여 코드를 구분합니다


### Step 3 – Leaving The Nest  

![](http://www.elecfreaks.com/estore/download/flappy-bird-5.png)
새의 형상을 만들었지만 아직은 움직일 수 없습니다.
먼저, y 좌표 바로 아래에 새로운 변수 '속도'를 추가해 보겠습니다.
display.clear ()를 while 루프로 이동하여 환영 메시지를 지우지 않고 새 위치가 매번 설정되기 전에 실행되는 새의 이전 위치를 지웁니다.
25-29행: '중력'을 기준으로 테두리 안에 새로운 y 좌표를 설정합니다 (최대 y = 99, 최소 y = 0).

while 루프에서 모든 것을 배치해야하는 이유는 무엇인가요? 
일정 밀리초마다 정확하게 새의 위치를 업데이트하여 블록이 반복될 수 있게 하려는 것 입니다.


### Step 4 – Defying Gravity

![](http://www.elecfreaks.com/estore/download/flappy-bird-6.png)

이제 우리는 A버튼을 눌러 새가 움직일 수 있게 해야합니다. 이 단계에서는 새가 지나간 벽의 수를 추적하는 새로운 '점수' 변수도 포함시킵니다. 버튼 B를 사용하여 언제든지 액세스 할 수 있습니다.
A의 키 누르기에 반응하려면 21행처럼 "button_a.was_pressed()"를 "fan_loop"아래에서 실행하세요. 반복하는 동안, A버튼을 누르면 새가 다시 올라오게 되고 하강 속도가 다시 빨라지게 됩니다. 
변수 '점수=0'을 추가하여 속도 및 y변수 아래에 새 변수 점수를 0으로 설정합니다. 코딩 습관으로 모든 변수를 한 곳에 설정하여 쉽게 따라 할 수 있도록 하는 것이 좋습니다.
버튼 A와 유사한 루프를 생성하여 버튼 B를 눌렀을 때 점수를 표시합니다. 표시(점수)는 원하는 시점에 점수를 표시합니다.

 
### Step 5 – Pipe Blaster  

![](http://www.elecfreaks.com/estore/download/flappy-bird-7.png)

make_pipe함수를 사용하여 첫번째 파이프를 만들 예정입니다! 그런 다음 변수 i에 할당하고 파이프를 표시합니다.
함수를 호출하면 코드 내의 전체 블록을 실행할 수 있습니다. 이를 통해 각 단계에서 하는 일을 더 쉽게 이해할 수 있습니다.
새 파이프를 만들기 위해 코드를 실행하는 함수 make_pipe()의 이름을 지정합니다. make_pipe()함수의 각 단계에서 수행되는 작업을 설명합니다.
19행에서는 defmake_pipe()를 사용하여 함수를 정의합니다.
20행에서는 각 좌표에 대해 밝기를 나타내는 '0'과 1행, 1열, 1열, 2열 등의 사용자 정의 이미지가 그려집니다. 
이렇게 하면 밝기가 4인 마지막 열의 LED가 켜집니다.
21 행에서 임의의 라이브러리를 사용하여 0과 3 사이의 난수를 호출합니다. 두 개의 홀을 폭발시키기 때문에 4를 사용하지 않습니다. 
즉 gap+1을 날렸기 때문이다. 만약 4가 선택된다면, 4열 5행에 구멍이 생길 것입니다. 그러나 5행이 없으므로 오류가 반환됩니다.
함수에 변수 i를 27행에 따라 할당해 봅시다. 이제 그 사이에 디스플레이를 추가하면 디스플레이에 파이프i가 표시됩니다.


### Step 6 – Frame Rate  

![](http://www.elecfreaks.com/estore/download/flappy-bird-8.png)

This step is where we set up the game constants. Here, the frame variable starts at 0, then increases by 1 every 20ms so it takes 400ms or 0.4s for the frames variable to increase by 20. Remember this, it’ll be easier for the incoming math. These constants aren’t used until Step 7, but let’s set them up first.
Line 15 just indicates the time taken (in ms) for frame to increase by 1, which is added as part of the while loop in line 37 (frame += 1). You can change the sleep(20) at the bottom of the code to sleep(DELAY) so it corresponds.
Line 16 sets the time taken for the wall to shift by 1 column. This is currently 0.4s or 20 frames.
Line 17 sets the time between the occurrence of another wall. This is currently 2.0s or 100 frames.
Line 18 sets the time between the score increasing. This should always be equivalent to the FRAMES_PER_NEW_WALL value so that each wall you pass is equivalent to one additional score.
To make the game harder, you would adjust these game constants, perhaps reducing the distance between each new wall for more walls (but change FRAMES_PER_SCORE to correspond to it). The game is currently set for one wall on the screen at any time, but you can definitely make it more chaotic by playing around with the values.
Note: The game constants are in uppercase, differentiating them from the other variables used. These are just [standard rules](https://www.python.org/dev/peps/pep-0008/) for Python programming. It’ll still work without following it, but your code should follow conventions to be readable.


### Step 7 – Pipe Dreams  

![](http://www.elecfreaks.com/estore/download/flappy-bird-9.png)
Here, we will compare the frame value with game constants to move the wall left, create a new wall and increase the score. This is all within the while loop so it’s checked every 20ms. Ready? Let’s go.
At this step, we’ll use the modulo sign (%). This provides the remainder when a number is divided by another number. So 4 % 2 returns 0 but 4 % 3 returns 3. Here, we’ll use it to check that the frame variable is equal to any of the game constants.
Moving wall left: Look at lines 65-67. This means the wall shifts when the frame is equal to 20, 40, 60… since they’re divisible by FRAMES_PER_WALL_SHIFT value of 20. You can vary this to make the walls move faster and increase the difficulty. Currently, the walls move every 0.4s.
Creating new wall: Look at lines 69-71. Every 100 frames, or 2 seconds, a new pipe is made by calling the make_pipe() function for i. This is the constant used to create and move the wall.
Increasing the score: look at lines 73-75. This means that a point is added when the bird travels for 2 seconds, or 1 wall. This value corresponds with the distance between walls so each wall passed is one point.
Game check: The game should be almost fully playable, with the welcome message, then the bird moving by pressing button A. You can see score with button B. There’s gravity acting on the bird so it falls down over time. Then the walls created randomly move right past it. Wow, you’re nearly done! Now, we just have to react to pipe collisions, ending the game and revealing the score when the bird collides with any pipe.


### Step 8 – Collision Course  

![](http://www.elecfreaks.com/estore/download/flappy-bird-10.png)

Phew, you made it to the last step! Ready to wing it? Now, we just need to add a collision reaction. This uses a get_pixel function that returns the LED brightness value at that position. ‘!=‘, the NOT function is also used. Let’s explain how it’s used below.
Add this collision checking code to the while loop, between the bird-drawing and wall-shifting. This means it checks for collision before new walls are created so there’s no extra scores by error.
As shown in line 66, we use an if loop. ‘i.get_pixel(1, led_y) != 0 checks if there is a pipe in the position of column 1 (where the bird is), specifically at led_y, the displayed position of the bird. If there is a pipe pixel in the same position as the bird’s coordinates, the i.get_pixel(1, led_y) returns 4, the brightness of the wall. This is NOT 0 so the function beneath, the collision checker, runs
Line 67-68 display the in-built sad face image for 0.5s. You can change how long this lingers, and to whatever other image you like. Python has a lot of images you can input. You can find the entire list [here](http://microbit-micropython.readthedocs.io/en/latest/tutorials/images.html).
Line 69 displays the score as a string, behind “Score”.
Line 70 ends the while loop so the game ends. This means that it’s ‘game over’.


### Start Game!  

And… that’s it! You’re done. Your game should be able to run and end, revealing the score at the end. It’s now a full-fledged frustratingly simple yet challenging game. Pat yourself on the back! That was a lot of hefty coding and new concepts. Look through your code, and try and figure out what each line. Add comments to explain it to yourself if necessary. This is a good practice for you to easily read your own code when coming back to it months later.

Good job! Have fun frustrating your friends with this novel interface for the annoying game. Now, you’re free as a bird to look for other projects, with a better understanding of the Python code.
Extension: Add a game loop, such that you can play again without resetting the device. I suggest changing the while loop’s requirements from True to a certain variable, a play_again function which can be changed with the press of a button. Look at other Python game loops for inspiration, like a scissors, paper, stone game.
