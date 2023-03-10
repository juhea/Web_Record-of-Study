# Web_Record-of-Study

Developer's first steps

------------------------------

##### 2023-02-11

## HTML에서는 TAG가 가장 중요한 핵심! 
* TAG : 설명하는 것 .. 열리는 태그, 닫히는 태그

* '<strong> .. </strong>' : 글씨를 진하게 강조
* '<u> .. </u>' : 밑줄
* '<h1> ~ <h6>' : ..뭐더라 :: 머릿글? 같은 느낌의 숫자가 커질수록 글자 크기는 작아짐
  
------------------------------
  
##### 2023-02-22
  
html new line tag : 줄바꿈 검색어
* '<br>' : 줄바꿈 ==> 닫는 태그가 없다.
* 장점 :  줄바꿈을 여러번 할 수 있다.

html paragraph tag : 단락 검색어
* '<p>' : 단락 ==> 단락을 나눌때 더 가치가 있다.
* 장점 : 어디서부터 어디까지가 단락이다, 라는 것을 표현할 수 있다. 
  => 시각적으로 부족한 부분은 css 를 통해서 훨씬 더 정교하게 제어할 수 있다.
* 단점 : 정해진 여백만큼만 벌어지게 되어있다. 시각적으로 자유도가 떨어진다.

##### 의미에 맞는 태그를 사용하는 것이 좋은 방법이다
(( 단락을 나눌땐, 여러개의 줄바꿈<br><br><br> <<<<<< 단락 표현<p> ))

#### css 에서.. (우리 수업과는 무관하기 때문에 몰라도 무관)
css에서 태그와 태그 사이의 여백을 나타내는 코드 
: 두 번째 태그에다가 <p style="margin"> 여백 
:: Ex) <p style="margin-top:40px;"> 윗 쪽 여백 40px


---------------------------------
  
https://opentutorials.org
예제 실습 사이트

----------------------------------
  
### # HTML이 중요한 이유
  
1. 검색엔진에 노출시킬 수 있다. 웹이 갖고있는 본래의 의미 : 정보라는 것을 탄탄히 하는것
2. 웹의 핵심적인 철학은 접근성 : 웹은 모든 운영체제에서 동작하고, 웹 페이지의 소스코드는 누구나 볼 수 있고, 웹은 저작권이 없는 순수한 공공재입니다.<br>
((( 개방성, 접근성 accessibility )))<br>
- 시각장애가 있는 분들을 배려하기위한 중요한 첫 출발은 문자를 시각화하여 예쁘게 꾸미기 보다는 <strong>HTML의 태그를 정확히 알고 의미에 맞게 사용하는 것!</strong>

  
---------------------------------

2023-02-23

< 최후의 문법 속성과 img >

- 이미지를 웹페이지에 포함시킬 때 사용하는 태그 : <img>
:: 어떤 이미지인지를 알려주기로 약속된 속성 = source :: <img src="웹브라우저에 적혀있는 주소">


@ Unsplash.com : 저작권에 구애받지 않고 사용가능한 고해상도 이미지 공유 사이트 @


<img src="coding.jpg"> 에서 크기를 조절하고 싶다? => <img src="coding.jpg" width="100%"> 
:: 자동으로 100% 크기에 맞게 이미지의 사이즈가 바뀌게 된다. Ex) width ="450" 도 가능


# img 문법 정리
	- 속성? : 태그가 태그만으로 의미가 부족할 때 이런 속성을 통해서 더 많은 의미를 부가할 수 있게 된 것이다.

 <img src="coding.jpg" width="100%"> 에서 src="coding.jpg" 과 width="100%" 은 속성, 영어로 Attribute라고 부른다.
: 속성의 위치는 상관이 없다.

---------------------------------

< 부모 자식과 목록 >

# 목차
<parent>
	<child></child>
</parent>

:: 이렇게 태그가 서로 포함 관계로 연관되어 있을 때, 포함하고 있는 태그를 부모 태그, 포함된 태그를 자식 태그라고 부른다.

- 목차를 쓸 때 사용하라고 고안해낸 태그 : 목록, 목차 : list : <li> </li>
: <ul> </ul> : Unordered List

@#@#@#@ 꿀팁 !!!! 여러줄에 한 번에 똑같은 태그를 넣고 싶을때는 Alt+줄 클릭 !!! @#@#
	:: 영상에서는 Ctrl 이라고 하는데 내 노트북에서는 안된다.. Ctrl과 Shift , Ctrl+Shift 도 해보고나서 Alt를 눌러 터득함, 안되는 이유는 모르겠다.

<ul>
	<li></li>
</ul>
:: ul => 부모, li => 자식

- 드래그 + Tab : 안쪽으로 들여쓰기 

# 즉 <li>와 같은 항목들은 그 항목이 어디서부터 어디까지가 서로 연관된 항목인지를 경계를 짓기 위한, 그룹핑을 하기 위한 부모 태그가 필요한 것이다.
=> * 자식 태그인 <li> 태그는 <strong>반드시</strong> 부모 태그를 갖고 있다! *
=> * 부모 태그인 <ul> 태그는 <strong>반드시</strong> 자식 태그를 갖고 있다! *

ㅋㅋㅋㅋㅋㅋㅋㅋ우리는 불행할 때ㅠㅠ 코딩을 하기 때문에 극단적 사고를 가져야한다(?)
1. ..
2. ..
3.. 
..
1억 ..
~ 되어있던것에서 제일 첫번째 줄을 없애줘! 하면 우린 1억개를 수정해야한다...... 
이럴땐? <ul>을 <ol>로 바꿔준다!!!!!!!!!!!

-목차, 목록같은 순차적인 숫자를 나타내주는 태그 : <ol> </ol> : Ordered List :


// <li>는 2대가 같이 다님 ( <ul> ) , 나중에 나올 <table>은 3대가 같이 다님 ( <tr>, <td>, </td>, </tr> )


---------------------------------

< 문서의 구조와 슈퍼스타들 >

- 웹 페이지 이름을 변경하는 방법 ( 웹 페이지 주소 아님, 헷갈리지 않기! )

웹 페이지의 제목을 사용자에게 명시적으로 알려줄 수 있을 뿐만 아니라 검색 엔진과 같은 기계들은 바로 이 <title>이라는 것을 책으로 치면 책 표지와 같은 정보로 사용한다.
* 그렇기 때문에 웹 페이지를 만들 때 <title>태그를 쓰지 않는 것은 손해다 !! *

- 웹 브라우저야 이 웹페이지를 열때는 UTF-8로 열렴
:: <meta charset="utf-8"> 을 title뒤에 작성
====> charset : character : 문자, set : 규칙
:: 'utf-8로 문서를 읽어라' 라는 규칙

------
################ 본문을 설명하는, 즉 바디를 설명하는 태그는 <head> 태그로 묶기로 약속함
<head>
<title> </title>
<meta charset="utf-8">
</head>

:  본문을 설명함 :: 즉 title이라는 태그는 본문의 제목이 무엇인지를 설명, 이 본문이 'utf-8'이라는 방식으로 저장되어있다를 설명

-----
###### 본문은 <body>라는 태그로 묶기로 약속함'
<body>
<ol>
	<li></li>
</ol>
<img sec="..">
</body>

: 본문

-------------

## 내가 생각하는 핵심 ! HTML에 있는 모든 태그는 <head>태그나 <body>태그 이 둘 중에 하나 아래에 놓이게 된다 !!!!!!!!!!!
=> <head>태그와 <body> 태그는 상당히 고위직 태그이다.*
==> 이 고위직 태그들을 감싸는 단 하나의 최고위층 태그가 있는데 그것은 바로 .. <html> </html>
Ex)
<html>

<head>
<title> </title>
<meta charset="utf-8">
</head>

<body>
<ol>
	<li></li>
</ol>
<img sec="..">
</body>

</html>

#### 중요 !!!!
:: <html> 위에 관용적으로 써주어야하는  ===>  <!doctype html>

--------------------

2023-02-26

< 14. HTML 태그의 제왕 >

Hyper Text 가 의미하는 태그 => <a> :: link 

사용 설명서를 찾을때 검색어 : 링크 : html specification
* 링크를 거는 태그 : <a> .. </a>
<a href="https://www.w3.org/TR/2011/WD-html5-20110405/">  ::: 이렇게 했을땐 링크를 누르면 그 창으로 바뀜
@ 여기에서 href란? hypertext의 첫글자 + 참조의 의미인 reference의 앞 세글자

@@ 새 창으로 띄우고 싶다 하면? target="_blank" 를 링크 뒤에 한칸 띄어쓰고 추가시켜줌
@@ 링크가 클릭하기전에 무슨 링크인지 툴팁으로 알려주고싶다? title="html5 speicification"
:: 마우스를 가져다대면 보인다. html5 speicification 이게 보임 !!

--------------------

2023-02-27

< 15. 웹 사이트 완성 >

웹의 가장 큰 제목을 <body> 다음에 작성 <h1>WEB</h1>

<body>
  <h1><a href="index.html">WEB</a></h1>
  <ol>  
    <li><a href="1.html">HTML</a></li>
    <li><a href="2.html">CSS</a></li>
    <li><a href="3.html">JavaScript</a></li>
  </ol>
..
</body>

--------------------

Ctrl-K,F : 선택한 영역 자동 코드 정렬 


Visual Studio Code에서 자동 줄맞춤을 하는 방법은 WIndows 기준으로
Ctrl + A로 전체 코드 선택 후 Ctrl + K + F 을 누르면 자동으로 줄 맞춤이 된다.

(Mac 단축키도 windows와 같은 command + K + F)

	
--------------------

	
2023-02-28

<16. 원시웹 > primitive web

웹의 고향은? 스위스

info.cern.ch : 웹의 메소포타미아

<img src="Web_메소포타미아.jgp">

--------------------

< 17. 인터넷을 여는 열쇠 : 서버와 클라이언트 >

컴퓨터 - 인터넷 - 컴퓨터
웹 브라우저(http://info.cern.ch/index.html) - 웹 서버 (http://info.cern.ch) (index.html)
정보 요청 request - 정보 응답 response
client - server
 
# 두 가지 방법
web hosting : 회사에 맡김
web server : 직접 설치하고 해봄

--------------------

< 18. 웹호스팅 : github page >

github 에서 repository 생성 후 파일 업로드 -> setting -> pages 
-> main or master branch .. save -> Repository의 Action에서 Page build and deployment 된거 확인 후
링크 클릭하면 웹 페이지 생성 완료 !!!!! 

# 중요 !!!! github에 index.html이라는 파일이 웹 페이지로 생성 되기때문에 파일명 고정 !!!!

--------------------

< 19. 웹서버 운영하기 VSCode Live Server >

* 비쥬얼스튜디오코드에서 확장 -> live server 설치 -> 우측 하단에 Go Live
실시간으로 변경이 되어서 Reload 할 필요가 없음

http://127.0.0.1:5500/index.html
Hyper  Internet  Port 
Text     Protocol
Transfer  Address
Protocol

Web browser -> 5500 Web Server
		6000 Game Server
		7000 Chatting Server

* 비쥬얼스튜디오코드에서 확장 -> ip address 설치 -> 우측 하단에 ip주소가 나옴

**** Go Live 누른 후 핸드폰에서 주소창에 컴퓨터 ip주소:5500 입력하면
핸드폰에도 웹 사이트가 뜬다!!! ****

--------------------

< 19.1.1 웹서버 운영하기 웹서버 소개>

Apache 사용해보기 !

검색어 추천 : how to install apache http server os

--------------------

< 19.1.2 웹서버 운영 윈도우 HTTP >

검색어 추천 : how to easy install apache on window
: bitnami wamp stack

나중에 bitnami wamp가 꺼져 있다면
C:Program Files:BitNami WAMPStack 에서 manager-windows.exe를 실행

화면에 표시되는 index.html 찾기
 : C:Program Files:BitNami WAMPStack:apache2:htdocs : index.html


http://127.0.0.1/index.html
::: Web Browser, Web Server : index.html

file:///C:/Program%20Files/BitNami%20WAMPStack/apache2/htdocs/index.html
::: Web Browser : index.html


--------------------


< 19.1.3 웹서버 운영 웹브라우저와 웹서버 통신 >

나의 IP 주소 찾기
: 설정 -> 상태 -> 네트워크 및 공유 센터 -> 이더넷
  
--------------------

2023-03-01

< 부록: 코드의 힘 : 동영상 삽입 >

@ 코드를 작성하다보면 긴 한 줄의 코드가 있다. 
이럴 때 자꾸 창을 넘어가서 자동으로 줄 바꿈을 해주고싶은데 기능을 못찾아서 애를 먹었다.
오늘 드디어 찾았다!!! Wordwrap 기능 : 줄 바꿈 여부를 제어합니다. : off->on으로 변경 @

- youtube 동영상 삽입 실습

<iframe  width="560" height="315" src="https://www.youtube.com/embed/4QCZxcCBtCI" title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen>
</iframe>

--------------------

< 부록: 코드의 힘 : 댓글 기능 추가 >

## 댓글 기능 추가하는 코드 ##

  <p>
    <div id="disqus_thread"></div>
<script>
    /**
    *  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
    *  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables    */
    /*
    var disqus_config = function () {
    this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
    this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
    };
    */
    (function() { // DON'T EDIT BELOW THIS LINE
    var d = document, s = d.createElement('script');
    s.src = 'https://web1-ia0he3iadr.disqus.com/embed.js';
    s.setAttribute('data-timestamp', +new Date());
    (d.head || d.body).appendChild(s);
    })();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
  </p>


--------------------

< 부록: 코드의 힘 : 채팅 기능 추가 >

https://www.tawk.to/

- Widget Code

<!--Start of Tawk.to Script-->
<script type="text/javascript">
var Tawk_API=Tawk_API||{}, Tawk_LoadStart=new Date();
(function(){
var s1=document.createElement("script"),s0=document.getElementsByTagName("script")[0];
s1.async=true;
s1.src='https://embed.tawk.to/63ff163131ebfa0fe7effd0c/1gqe6tcsc';
s1.charset='UTF-8';
s1.setAttribute('crossorigin','*');
s0.parentNode.insertBefore(s1,s0);
})();
</script>
<!--End of Tawk.to Script-->

# 짱 재밌다!!!!!!! 웹 사이트에서 방문자가 실시간 채팅을 하면 tawk에서 답장한다 !!! #

--------------------


##### 2023-03-05 

< 부록: 코드의 힘 : 웹사이트 방문자 분석기 >

https://analytics.google.com

수동으로 Google 태그 설치
아래에 이 계정의 Google 태그가 있습니다. 태그를 복사한 후 웹사이트의 각 페이지 코드에서 <head> 요소 바로 다음에 붙여넣으세요. 
Google 태그는 각 페이지에 하나씩만 추가합니다.

<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-ZGPVS6TRBT"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-ZGPVS6TRBT'); 
</script>

//  gtag안에 'G-ZGPVS6TRBT' 이 부분은 변경되는 부분
- 보고서 - 실시간 :: 방문자 확인 가능

Audience-Geo-Language :: 한국어가 압도적으로 많은 걸 볼 수있다.

- 웹사이트 방문자 분석기를 활용해서 나의 인스타그램을 웹사이트로 활용해보았다!
https://juhea.github.io/ju_nye_instagram/




-----------------------------
	
참조 : Egoing Lee :: https://www.inflearn.com/course/%EC%BB%B4%ED%93%A8%ED%84%B0-%EC%9B%B9-%EC%BD%94%EB%94%A9-%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D-%EC%8B%9C%EC%9E%91-web-1/dashboard
	
	
