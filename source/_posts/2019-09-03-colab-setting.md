---
layout: post
title:  "쉽게 따라하는 Colab과 구글 드라이브 연결"
date:   2019-09-03
excerpt: "Colab에서 구글 드라이브를 저장소로 사용하는 방법에 대해 알아봅시다."
sitemap :
  changefreq : daily
  priority : 1.0
setting: true
tag:
- Setting
- colab
- python
- gpu
comments: true
---

오늘 포스팅은 그림이 무척 많은 `Colab`을 사용하는 방법부터 `Colab`에서 `구글 드라이브`를 저장소로 사용하는 방법입니다. 차근차근 따라와 주세요.

먼저 구글 드라이브에 들어가주세요. 저장소로 쓰기 때문에 어느 정도 용량확보가 필요합니다. 그래서 기존 구글 계정의 용량이 모자른다면 새로운 구글 계정을 만드셔서 하시는 것을 추천합니다. 

---

## Index

<a href="#01">1. Colab 추가하기</a>  
<a href="#02">2. Colab 시작하기</a>  
<a href="#03">3. GPU 사용하기</a>  
<a href="#04">4. Google Drive 연결하기</a>  

---

<a id='01'></a>

### 1. Colab 추가하기

<img src = "https://sihan-son.github.io/public/colab/1.png">

구글 드라이브의 메인 화면에서 마우스 우클릭을 해주시면 위와 같은 이미지가 뜨게 됩니다. 저는 이미 `Colab`을 추가한 상태라 항목에 `Colab`이 보이지만 이 글을 보고 계신 대부분의 사용자 분들은 없는게 정상이니 걱정하지 마세요.  

`Colab`이 항목에 없으시면 제일 아래 보이는 `연결할 앱 더보기`를 눌러 주세요. 그러시면 아래와 같은 창이 뜨게 됩니다.

<img src = "https://sihan-son.github.io/public/colab/2.png">  

위의 창은 `Colab`을 검색해서 나온 결과입니다. 처음하시면 `평가하기`버튼 대신에 `연결하기`를 눌러주시면 `Colab`이 연결됩니다. 

<a id='02'></a>

### 2. Colab 시작하기

이제 `Colab`을 첫번째 이미지에서 처럼 마우스 우클릭 하고 `Google Colab`을 눌러주시면 됩니다. 그러면 다음과 같은 화면이 반겨줍니다.

<img src = "https://sihan-son.github.io/public/colab/3.png">

이제 여기서 그냥 코딩을 하시면됩니다. 기본적인 사용법은 `Jupyter Notebook`과 동일한데 단축키에 차이가 있습니다. 이건 별도의 포스팅으로 찾아뵙겠습니다. `Colab`은 이렇게 사용하면 되는데 이렇게만 쓸거면 로컬에서 `Jupyter`, `PyCharm`등을 쓰는게 나을테니까 우리가 `Colab`을 쓰는 이유인 `GPU`연결에 대해서 알아보겠습니다. 


### 3. GPU 사용하기

<a id='03'></a>

<img src = "https://sihan-son.github.io/public/colab/4.png">  

<img src = "https://sihan-son.github.io/public/colab/5.png">  

하드웨어 가속기를 기본 `CPU`로 되어 있는 것을 `GPU`로 바꿔주시면 됩니다. 주의하실 점은 `TPU`도 있는데 `TPU`도 속도는 빠르지만 `GPU`와는 코드 작성법이 좀 다르기 때문에 지금은 `GPU`를 선택해 주시면 됩니다. `GPU`를 사용하시면 세션이 12시간 제한이 있기 때문에 주의하면서 사용해주세요. 중간중간 세션이 끊길 수도 있기 때문에 확인해주셔야 해요.



### 4. Google Drive 연결하기

<a id='04'></a>


<img src = "https://sihan-son.github.io/public/colab/6.png">

왼쪽에 있는 빨간 동그라미를 눌러주세요

<img src = "https://sihan-son.github.io/public/colab/7.png">

왼쪽의 3개 메뉴 중에서 파일을 눌러주세요.

<img src = "https://sihan-son.github.io/public/colab/8.png">

파일에서 드라이브 마운트를 눌러 주시면 화면처럼 우측에 저런 코드가 자동적으로 작성됩니다.

<img src = "https://sihan-son.github.io/public/colab/9.png">

저 코드를 실행 시켜 주시면 `URL`과 입력창이 뜨게 되는데 구글 드라이브 사용을 위한 인증 절차 입니다.

<img src = "https://sihan-son.github.io/public/colab/10.png">

이렇게 되면 연결이 성공되었습니다. 