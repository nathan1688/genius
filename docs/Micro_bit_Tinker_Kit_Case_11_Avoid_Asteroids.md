Micro : bit에서 자신 만의 작은 아케이드 게임을 만들고, 5 x 5 해상도의 매력을 느껴보십시오!
이 메뉴얼은 Raffles Institution의 Josh Ho가 기고했습니다.

## 단계 0 - 사전 빌드 개요
---
이 프로젝트에서는 Micro : bit와 ADKeyboard 만 사용하여 Raiden-esque 게임을 만들 계획입니다. 이 게임의 목적은 가능한 한 오랜 시간 동안 게임이 진행되는 동안 속도가 증가하는 들어오는 발사체를 피하는 것입니다. Micro : bit LED가 화면에 표시되고 ADKeyboard가 컨트롤러가됩니다.


## 재료 :
---
- 1 x [BBC Micro : bit] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 마이크로 USB 케이블 1 개
- 1 x [브레이크 아웃 보드] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 x [ADKeyboard] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)

팁 : 위의 모든 구성 요소를 원하면 [ElecFreaks Micro : bit Tinker Kit] (http://www.icbanq.com/shop/templete_list.asp?t_idx=163)가 필요할 수 있습니다.

![](https://i.imgur.com/Mp5cNkJ.jpg) 


목표 :
---
- Micro : bit로 간단한 게임을 만드십시오.
- 고급 프로그래밍 로직을 학습합니다.
- 스프라이트로 실험 해보세요.


### 1 단계 : 구성 요소
ADKeyboard는이 프로젝트의 유일한 외부 구성 요소입니다. ADKeyboard를 연결하기 전에 브레이크 아웃 보드에 Micro : bit를 삽입하기 만하면됩니다. 전선의 색상이 핀의 색상과 일치하는지 확인하십시오. 아주 간단합니다!

![](https://i.imgur.com/SbMCZYA.jpg)  

### 2 단계 : 사전 코딩
우리는 키트 구성 요소를 사용할 수 있도록 코드 패키지를 추가 할 것입니다. 코드 드로어에서 "고급"을 클릭하면 더 많은 코드 섹션을 볼 수 있으며 "패키지 추가"에 대한 코드 드로어의 하단을 볼 수 있습니다.

![](https://i.imgur.com/TCRoSBR.jpg)

그러면 대화 상자가 열립니다. "팅커 키트"를 검색 한 다음 패키지를 클릭하여 패키지를 다운로드하십시오.

![](https://i.imgur.com/8a7kDKF.png)

참고 : 비 호환성 문제로 인해 일부 패키지가 제거 될 것이라는 경고 메시지가 표시되면 프로젝트 파일 메뉴에서 프롬프트를 따르거나 새 프로젝트를 만들어야합니다.

### 3 단계 : 코딩
변수를 사용하여 프로그램에 데이터를 저장할 수 있습니다. 점수를 게임에 저장하는 데 사용합니다.

![](https://i.imgur.com/IpUHtHw.jpg)

마이크로 : 비트 (버튼 B)에있는 버튼을 사용하여 게임이 진행되지 않을 때 최고 점수를 표시합니다. "On button B pressed"코드 블록이이 조건을 충족하며 해당 블록 내에서 "highscore"변수가 표시됩니다.

![](https://i.imgur.com/koVaer9.jpg)

우리는 카운트 다운을 시작하는 게임을 시작하는 버튼을 사용합니다. 어떤 일이 일어나기 전에 우리는 게임에서 스프라이트를 초기화해야합니다. 스프라이트는 기본적으로 마이크로 : 비트 화면의 단일 LED로 표시되는 엔티티입니다. 그들은 MakeCode에서 제공되는 코드 블록을 사용하여 이동하고 방향을 바꿀 수 있습니다. 또한 플레이어가 아직 살아 있는지 여부를 나타내는 "alive"변수와 발사체의 이동 속도를 결정하는 "speed"변수를 초기화합니다. 카운터 직관적으로 숫자가 낮을수록 발사체가 더 빠르게 움직입니다.

![](https://i.imgur.com/WS9mJfW.jpg)

다음으로 while 루프를 추가합니다. while 루프는 지정된 조건이 충족되는 한 반복적으로 실행됩니다. 이 경우 플레이어가 아직 살아있을 때에 만 게임이 계속 실행됩니다.

![](https://i.imgur.com/lkr8BiI.jpg)

참고 : 여기에주의하십시오! 왜냐하면 while 루프는 Micro : bit를 크래시 할 가능성이 있기 때문입니다.

루프 내에서 게임 제어를 제어하는 ​​코드 그룹 인 ADKeyboard를 추가합니다. 빨간색 A 버튼을 누르면 스프라이트가 왼쪽으로 이동합니다. 빨간색 B 버튼을 누르면 스프라이트가 오른쪽으로 이동합니다. 파란색 D 버튼을 누르면 게임이 즉시 중지됩니다.

![](https://i.imgur.com/eLMZEwI.jpg)

그 후, 우리는 적의 발사체의 움직임을 규정 할 것입니다. 먼저 Math 모듈에서 임의 블록을 선택하여 난수를 선택합니다. 이 숫자는 어느 발사체가 1 씩 위로 움직이는지를 결정합니다. 그러나 발사체가 맨 아래 줄에있는 경우 발사체의 동작을 결정하는 더 많은 코드가 있으므로 발사체가 맨 아래 줄에있는 경우에만 적용됩니다.

![](https://i.imgur.com/4WWoybd.jpg)

이 비트는 이미 움직일 때 발사체의 동작을 코드합니다. 중간 세 행에 있으면 1 씩 이동하고, 맨 위 행에있는 경우 맨 아래 행으로 돌아갑니다.

![](https://i.imgur.com/pvmKWJo.jpg)

우리는 또한 스프라이트가 플레이어를 만지기 때문에 플레이어가 언제 타격되는지 알 수 있어야합니다. 플레이어가 히트하면 "살아있다"라는 변수가 "거짓"으로 바뀌고 while 루프는 루핑을 멈추고 게임도 멈춥니다.

![](https://i.imgur.com/z21zJtA.jpg)

마지막으로, 매 루프마다 점수가 1 씩 증가합니다. 획득 한 15 점마다 "속도"가 40만큼 감소하여 발사체의 속도가 빨라집니다. 일시 정지는 발사체의 속도를 제어합니다.

![](https://i.imgur.com/car77QA.jpg)

게임이 끝나면 스프라이트가 삭제되어 LED 스크린이 막히지 않도록해야합니다.

![](https://i.imgur.com/I7IDuAL.jpg)

게임은 LED 스크린에 "Game Over"를 표시하고 점수를 얻습니다. 점수가 현재 최고 점수보다 높으면 최고 점수가 대체됩니다.

![](https://i.imgur.com/0YPq5ha.jpg)

이 코드를 직접 입력하지 않으려면 아래 링크에서 전체 프로그램을 다운로드 할 수 있습니다.

[https://makecode.microbit.org/_My0Mas61bbaU](https://makecode.microbit.org/_My0Mas61bbaU)  

또는 아래 페이지에서 다운로드 할 수 있습니다.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_9Hz86C6XzbYx" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>


### 4 단계 - 성공!
올레! Micro : bit로 미니 비디오 게임을 만들었습니다. 이제 친구들과 함께 요!
