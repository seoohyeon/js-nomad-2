# 자기소개 웹페이지 작성 목표
최대한 간결하면서 핵심적인 요소가 눈에 잘 띄도록, 

최신 감각을 잃지 않고 부드러운 인상을 줄 수 있는 페이지를 만들어야겠다고 생각했습니다.

그래서 내가 누구인지, 나의 소개글, 18주 간의 계획을 한눈에 나타내기 위해

이미지와 그림을 적극 활용하였습니다.


# 목표달성 과정 중 어려운 점 및 극복 방법
진행 과정에 있어, 

초반에 디자인 컨셉이 생각만큼 나오지 않아 많이 고민하고 힘들었습니다.

또한, 각 요소들을 div로 감싸고 정렬을 해야하는데 

바로 정렬했을 때 원하는 방향의 결과물이 나오지 않아 시간을 많이 소비하였습니다.

하지만, 예전에 제가 공부하고 까먹은 부분들이라 

제 블로그에 찾아가 다시 보완하여 나타낼 수 있었고 

멋쟁이사자처럼 홈페이지를 연구해보며 사용자환경에 맞는 디자인을 구축해볼 수 있었습니다.


# 목표 달성도와 보강하고 싶은 점
자기소개 웹페이지는 앞서 계획한 목표의 80%정도가 구현되어 진 것 같습니다.

전체적으로 margin, padding, flex를 이용하여 정렬하려 했지만,

시간이 부족한관계로 원하는만큼 깔끔한 정렬 및

사용자가 조절하는 웹페이지 크기에 따른 페이지 구성 정렬을 완벽히 하지 못한 점,

조금 더 역동적인 웹페이지를 만들지 못한 점에 대해 부족함과 아쉬움을 느낄 수 있었습니다.


# HTML/CSS 기술 중심 구현 설명
## 1. who is 김서현 부분
   ![a_tag](https://user-images.githubusercontent.com/38703262/202440664-ddde6202-b1ce-4396-87bb-a8aa56dba622.png)<br>
![a_tag_css](https://user-images.githubusercontent.com/38703262/202440717-63ac1141-1a53-411b-8e00-2f046fb9019d.png)<br>
저의 정보들이 들어가있고, 각각의 주소는 a태그로 링크를 걸었습니다.

사용자 환경을 생각하여, 

hover로 마우스커서 이동시 url에 line이 생기고 초록색으로 바뀌게 하고 

active를 이용하여 클릭시에는 line이 사라지고 빨간색이 나타나도록 하였습니다.

각각은 모두 현재페이지가 아닌 새로운 창을 생성하여 이동하게 되므로, 

현재 페이지는 그대로 남아있습니다. a태그에 target에 _blank 를 주어 나타낼 수 있었습니다.


## 2. Introduction 부분 
3가지 그림으로 저를 표현하였습니다.<br><br>
    ![intro_1](https://user-images.githubusercontent.com/38703262/202440726-66dbedbf-c323-43f9-8e22-f4c62cc8c725.png)<br>
![intro_2](https://user-images.githubusercontent.com/38703262/202440765-c7d568a7-4f13-4bbc-9b9a-30a13deebdbb.png)<br>
그림에 마우스를 올리면, hover를 이용하여 처음에 숨겨진 설명글이 보이도록 하였고, 

position: absolute를 주어 설명글창과 이미지가 겹치게 처리하였습니다.

각각의 그림들을 누르면 세부적인 설명을 볼 수 있는 새 창으로 이동합니다.
![intro_3](https://user-images.githubusercontent.com/38703262/202440764-95e8d70e-575c-47db-9146-1340dac3e3a4.png)<br>

html로 각 페이지들을 만들어 a태그로 연결시켜 주었습니다.

연결된 페이지들에서는 모두 이미지를 배경으로 하였는데, 

이미지가 반복되지 않기 위해 no-repeat을 해주었고 화면에 다 차도록 하였습니다.

KSH2.css 파일을 따로 만들어서 꾸며주었고 

통일성을 위해 3가지 html의 class명이 같도록 지정하고, 모두 KSH2.css를 이용하였습니다.


## 3. 18 Weeks Plan 부분

### 3-1. 계획 요약정리
![plan_1](https://user-images.githubusercontent.com/38703262/202440761-dcf90c81-e900-4bbb-afab-a033fa99673f.png)
![plan_2](https://user-images.githubusercontent.com/38703262/202440778-67afbeec-d710-44ce-9c45-78068e9d3386.png)

한눈에 저의계획을 요약하여 드러내고자

div를 이용해 계획을 데이터 이미지화 시켰습니다.

앞서 말씀드린 부드러운 인상을 위해 모두 border-radius:25px로 주었고

글자가 중간에 오도록 하기위해 flex를 주고

justify-content, align-items 모두 center로 이용하였습니다.

div전체의 class에 공통된 모든 속성을 주었고 나머지는 각각 속성을 주기위해

:nth-chlid(숫자)를 이용하였습니다.<br><br>

### 3-2. 계획 Open/Close 기능
![plan_3](https://user-images.githubusercontent.com/38703262/202440775-92d87bef-5310-4f2e-821b-e40abb95bf9d.png)
![plan_4](https://user-images.githubusercontent.com/38703262/202440773-8eac29d4-7511-47c5-9b6b-19df169ff6dd.png)<br>
또, 계획의 구체적인 설명이 너무 길다보니, js없이 펼쳤다 숨겼다 하기위하여

라디오헤드 checkbox를 이용하였습니다.

input의 type을 checkbox을 생성하고 그 후 그 checkbox모양을 display:none으로 숨깁니다.

그리고 처음페이지는 열려있길 원했기 때문에 checked:checked'로 설정해주었습니다.

그 라디오헤드버튼이 checked된 상태에서는 details가 보이도록 하기위해

#check-btn:checked ~ .details에서 display:block을 해주었습니다.

display: none 처리된 버튼이 안보이는 Input 태그를 클릭하기 위해 

label 태그를 추가하여 클릭이 용이하게 해주고 

속성으로 for에 input에 대한 name을 추가했습니다.

그래서 label을 클릭할 때마다 계획설명글(details)이 사라졌다 보였다 반복합니다. <br><br>
<
### 3-3. 좌우이동 Animation
![plan_5](https://user-images.githubusercontent.com/38703262/202440768-8ffdddd5-2707-40a5-b282-f9ec8277291c.png)<br>
마지막에는 움직임을 주고 싶어, 애니메이션을 이용하였습니다.

keyframes에 애니메이션 이름과 움직임 동작을 지정해주었습니다.

간단하게 좌우로 왔다갔다 하기위해 left 20% ~ 60%로 해주었고

애니메이션 지속시간은 3초, 무한반복, 방향은 갔다가 반대로 가도록 하였습니다.

또, 오른쪽 아래에는 div로 top기능을 만들어 웹페이지 가장 상단으로 갈 수 있도록 하였습니다.<br><br>


## 4. footer 부분

간단한 구분기호를 위해 hr로 선을 그엇고

기본적인 홈페이지에 다 작성되는 copyright를 작성하여 

제대로된 웹페이지의 마무리를 하도록 하였습니다.
