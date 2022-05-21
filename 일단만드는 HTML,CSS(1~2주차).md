# HTML/CSS

HTML/CSS로 만드는 나만의 이력서

## HTML
<<<<<<< HEAD

대제목을 `TAG`라고 한다

<가방2><가방1>내용물입니다. </가방1></가방2>

태그로 감싼다.

<h1> heading 1 </h1>

<p> 본문

=======
>>>>>>> a73f0cc3a39e73a0c16a7e0a43ddc3c384ebeed5
많이 쓰이는 태그를 이용해서 쉽고 간결하게 코드를 짠다.
```
<가방2><가방1>내용물입니다.</가방1></가방2>
```
컨텐츠를 `TAG`로 감싼다.
```
<h1> h1(heading1) </h1>
```
```
<p> p(본문) </p>
```

```
<!DOCTYPE html>
<HTML></HTML>
```
없어도 동작은 하지만, 반드시 명시한다.

```
<head></head>
```
내용물에 대한 추가적인 정보가 담겨있음

```
<meta charset=”UTF-*”>
```
한글이 정상적으로 출력되게 하는 코드

```
<title></title>
```
문서의 제목을 만드는 태그

```
<link rel=”stylesheet” href=codelion.css”>
```
단독태그(css파일과 연결)

```
<body></body>
```
컨텐츠 내용이 담겨있음

```
<section></section> <article></article>
```
div와 완전히 똑같음(html문서를 꾸미기 위해 분리)

```
<footer></footer>
```
하단에 표시하는 안내문

```
<img src=”이미지 경로”> 
```
이미지띄우기

```
<a href=”주소”> </a>
```
하이퍼링크

lorem ipsum : 의미없는 텍스트(디자인을 보기 위해 사용)

## CSS
```
footer {

text-align : center;

}

p {

text-align : center;

color : orange;

}

.big-font {

font-size: 40px;

}

.small-font {

font-size: 15px;

}
```
이런 식으로 쓴다

class 지정하는법
```
<p class=”big-font”>

<div class=”mainbox”>
```
border: 두께 방식 색깔;

width: 두께;

padding: 테두리와 content 사이의 폭

margin: 상자 밖 영역

text-align: center; //글씨를 가운데 정렬

margin-left: auto;

margin-right: auto; //div를 가운데 정렬

box-shadow: 가로축 세로축 흐린정도(블러) 퍼진정도(스프레드) rgba( , , ,투명도)

//박스에 그림자 생성

```
@import url('https://fonts.googleapis.com/css?family=Montserrat:100,200,300,400,500,600,700,800&display=swap'); 
```
구글 웹폰트를 불러온다

- { //모든 내용에 적용

  font-family: ‘Montserrat’;

}

font-size

font-weight: bold light lighter;

font-style: italic;

border-bottom: 1px solid #ebebeb; (아래에만 선을 준다)

margin-bottom:

padding-bottom: //아래에만 마진과 패딩을 준다

line-height: 16px; //줄간격

float: left(왼쪽으로 떠다님)

right(오른쪽으로 떠다님)

overflow: hidden;

//float로 띄운 컨텐츠들을 묶고 다른 컨텐츠가 이 컨텐츠의 영향을 받지 않게함
