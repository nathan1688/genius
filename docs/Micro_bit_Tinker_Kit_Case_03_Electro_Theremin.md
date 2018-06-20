

![](https://i.imgur.com/TJvoaaV.jpg)

## Goals
---

- 마이크로비트를 이용해 아날로그 센서를 사용하는 법.


## Materials
---

- 1 x [BBC 마이크로비트](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 1 x Micro USB cable
- 1 x [부저모듈](http://www.icbanq.com/shop/templete_list.asp?t_idx=163)
- 2 x F-F 점퍼 케이블
- 1 x 가변저항


## Procedure  
---

### Step 1

부저 모듈을 Pin0에 연결해주세요. positive 리드핀이 노란색 신포 핀에 연결되고 negative 리드핀이 센서비트보드의 검은색 접지 핀에 연결되어 있는지 확인해 주세요.
가변저항을 Pin1에 연결해주세요. 색상에 따라 연결하시면 됩니다. 센서비트 보드의 케이블 색상과 가변저항의 케이블색상을 일치하여 연결해주세요.

![](https://i.imgur.com/PUPIRol.jpg)

### Step 2

Makecode에서는 변수를 사용하여 전위차계의 값을 추적합니다. 여기서 변수는 변화하는 값을 저장할 수 있는 그릇과 같습니다.
Variable 카테고리에서 reading이라는 새로운 변수를 만들어 주세요.
이번 프로젝트에서는 변수를 디지털 대신 가변저항의 아날로그 값으로 설정하려고 합니다.
아날로그 값을 읽으면 디지털 1 또는 0 대신 가변저항에서 모든 신호 범위에 액세스 할 수 있습니다. Pins 카테고리에서 찾아 추가 할 수 있습니다.

![](https://i.imgur.com/DMXaJD9.png)

### Step 3

변수의 수를 표시하여 가변저항의 최소값과  최대 값을 확인하세요.
노브를 반 시계 방향으로 돌리면 최대한 작아지며 시계 방향으로 돌리면 최대가 됩니다.
값이 어떻게 변화하는지 주의해 주세요. 이것은 마이크로비트가 화면 전체에 걸쳐 큰 숫자를 스크롤하는데 시간이 걸리므로 새로운 값을 읽을 때 가변저항의 숫자가 변할 수 있습니다.

![](https://i.imgur.com/eNZiQx8.png)

### Step 4

이제 우리는 가변저항에서 읽은 값을 사용하여 변수에 배치할 것입니다.
아쉽게도 마이크로비트의 음악 블록은 가변저항만큼 넒은 범위를 설정 할 수 없습니다. 이러한 경우, 가장 높은 가변저항 값이 우리가 지정하고자 하는 가장 높은 음과 일치하는지 확인해야 합니다.
마이크로비트 피아노 키에서 사장 낮은 음과 가장 높은 음의 값을 확인하세요.
핀 카테고리의 맵 블록을 사용하여 모든 값을 입력하세요.

![](https://i.imgur.com/WF67giW.png)

### Step 5

이전 단계에서 not라는 변수를 만들었습니다. note 변수를 매핑 된 값으로 설정했는지 확인해 주세요. note 변수를 사용하여 톤을 울립니다. 이코드를 마이크로비트에 저장하면 음을 낼 준비가 완료된 것입니다.

![](https://i.imgur.com/laFfa5r.jpg)

코딩을 직접 하는것을 원하지 않는다면, 아래의 링크를 통해 다운로드하여 사용해주세요.

[https://makecode.microbit.org/_5jUeetL6oKqi](https://makecode.microbit.org/_5jUeetL6oKqi)

또는 아래 페이지에서 다운로드 할 수 있습니다.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_5jUeetL6oKqi" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>


### Cool Stuff!

이번 프로젝트에서는 가변저항을 사용하는 방법에 대해서 배웠습니다. LED, 서보모터 및 기타 구성 요소를 제어하는 데 사용할수 있습니다!

