# HTML
>출처 : [developer.mozilla.org](https://developer.mozilla.org/ko/docs/Web/HTML)


- Hypertext Markup Language
- 웹을 이루는 기초요소, 웹 컨텐츠의 구조를 정의(구조화)할 때 사용.
	- 웹 브라우저에 글, 이미지 등의 다양한 컨텐츠를 \<태그> 형식의 마크업 언어로 표현.

## Syntax
- 대소문자를 구분하지 않고, 혼용도 가능.
- 일반적으로 \<tagName>content</tagName>의 형식으로 사용한다.
- 예외적으로 단일태그, \<tagName /> 혹은 \<tagName> 형식으로 사용되는 요소도 있다.
- 태그 내부에는 속성값이 들어갈 수 있다. ex) \<tagName attributeName="value">
- 속성값은 다중 적용 가능하다.

## Display Categories
- CSS의 적용 등, content의 출력 방식을 바탕으로 분류가 가능하다.
1. block
	- 부모 요소의 전체 공간을 차지한다.
	- 언제나 새로운 줄에서 시작, 좌우 양쪽의 모든 공간을 차지한다.
	- \<body> 요소에서만 사용 가능하다.
	- block 내부에는 block과 inline 모두 중첩이 가능하다.
	- 예외적으로 block 중 \<p> 태그는 inline만 중첩 가능하다.
2. inline
	- 컨텐츠의 흐름에 따라, 태크에 할당된 공간만을 활용한다.
	- 새로운 줄을 생성하지 않아도 어디서나 시작 가능하고, 필요에 의해서만 공간을 차지한다.
	- inline 내부에는 inline만 중첩이 가능하다.
	

## Comments
- 화면에 보이지 않고 source code 안에 텍스트를 남기기 위한 용도로 사용한다.
- \<!-- content --> 의 형식으로 사용한다.


## Tags <span id="linkTest"></span>

### \<!DOCTYPE html>
- DOCTYPE은 HTML이 지켜야할 규칙에 대한 연결부? 같은 역할을 했다.
- 현재는 단지, 올바른 구동을 위한 규칙과 같은 선언으로 쓰인다.


### \<html>\</html>
- 전체 페이지를 감싸는 root 역할의 요소.


### \<head>\<head/>
- 페이지에 포함되어 있는 모든 숨겨진 내용들을 담고 있는 컨테이너.
- CSS, 문자 집합의 선언, 페이지에 대한 설명, 검색에 노출될 키워드 등... 페이지에 대한 모든 내용을 가진다.
#### \<meta /> 
- 단일태그


### \<body>\</body>
- 


### \<script>\</script> : inline


### \<style>\</style>


### \<div>\</div> : block
- 

### \<span>\</span> : inline




### \<h1>\</h1> ~ \<h6>\</h6> : block
- <h1>제목, 숫자가 작을수록 메인 제목에 가깝다.</h1>
- <h2>제목, 숫자가 작을수록 메인 제목에 가깝다.</h2>
- <h3>제목, 숫자가 작을수록 메인 제목에 가깝다.</h3>
- <h4>제목, 숫자가 작을수록 메인 제목에 가깝다.</h4>
- <h5>제목, 숫자가 작을수록 메인 제목에 가깝다.</h5>
- <h6>제목, 숫자가 작을수록 메인 제목에 가깝다.</h6>

```
- <h1>제목, 숫자가 작을수록 메인 제목에 가깝다.</h1>
- <h2>제목, 숫자가 작을수록 메인 제목에 가깝다.</h2>
- <h3>제목, 숫자가 작을수록 메인 제목에 가깝다.</h3>
- <h4>제목, 숫자가 작을수록 메인 제목에 가깝다.</h4>
- <h5>제목, 숫자가 작을수록 메인 제목에 가깝다.</h5>
- <h6>제목, 숫자가 작을수록 메인 제목에 가깝다.</h6>
```


### \<p>\</p> : block
- <p>문단</p><p>나누기</p>

```
- <p>문단</p><p>나누기</p>
```

### \<br/> : inline
- 단일태그
- 줄<br/>바꿈

```
- 줄<br/>바꿈
```


### \<b>\</b> : inline
- bold, 텍스트를 <b>굵게</b> 표시.
- 중요 X, 일반 텍스트와 표시만 다를 뿐 <b>동일</b>하게 취급.

```
- bold, 텍스트를 <b>굵게</b> 표시.
- 중요 X, 일반 텍스트와 표시만 다를 뿐 <b>동일</b>하게 취급.
```


### \<strong>\</strong> : inline
- 텍스트를 <strong>굵게</strong> 표시.
- 일반 텍스트에 비해 해당 content의 <strong>중요함</strong>을 알리는 용도 포함.

```
- 텍스트를 <strong>굵게</strong> 표시.
- 일반 텍스트에 비해 해당 content의 <strong>중요함</strong>을 알리는 용도 포함.
```

### \<i>\</i> : inline
- italic, 텍스트를 <i>기울어지게</i> 표시.
- 중요 X, 일반 텍스트와 표시만 다를 뿐 <i>동일</i>하게 취급.

```
- italic, 텍스트를 <i>기울어지게</i> 표시.
- 중요 X, 일반 텍스트와 표시만 다를 뿐 <i>동일</i>하게 취급.
```


### \<em>\</em> : inline
- italic, 텍스트를 <em>기울어지게</em> 표시.
- 일반 텍스트에 비해 해당 content의 <em>중요함</em>을 알리는 용도 포함.

```
- italic, 텍스트를 <em>기울어지게</em> 표시.
- 일반 텍스트에 비해 해당 content의 <em>중요함</em>을 알리는 용도 포함.
```

### \<ins>\</ins> : inline
- <ins>밑줄</ins>을 표시.

```
- <ins>밑줄</ins>을 표시.
```


### \<u>\</u> : inline
- 밑줄, 하지만 CSS로 표현하는 걸 권장.



### \<del>\</del> : inline
- 텍스트 중앙에 <del>취소선</del>을 표시.

```
- 텍스트 중앙에 <del>취소선</del>을 표시.
```


### \<s>\</s> : inline



### \<mark>\</mark> : inline



### \<sup>\</sup> : inline
- 위첨자


### \<sub>\</sub> : inline
- 아래첨자




### \<q>\</q> : inline
- <q>짧은 인용문에 사용.</q>

```
- <q>짧은 인용문에 사용.</q>
```


### \<blockquote>\</blockquote> : block
<blockquote>내용이 긴(블록) 인용구에 사용한다.</blockquote>

```
<blockquote>내용이 긴 인용문에 사용한다.</blockquote>
```


### \<cite>\</cite> : inline


### \<small>\</small> : inline



### \<abbr>\</abbr> : inline
- 준말 혹은 머릿글자 등을 표현하기 위해 사용.


### \<code>\</code> : inline
- 컨텐츠 내부에 짧은 코드 내용을 삽입할 때 사용.


### \<pre>\</pre> : block
- 텍스트를 입력값 그대로 표현하기 위해 사용.


### \<kbd>\</kbd> : inline
- 키보드 입력값을 표현할 때 사용.


### \<var>\</var> : inline
- 변수명 표현.


### \<data>\</data> : inline


### \<time>\</time> : inline


### \<progress>\</progress> : inline



### \<meter>\</meter> : inline


### \<hr> : block
- 단일태그
- 장면의 전환, 구획의 분리 등을 표시하기 위해 사용.

### \<ul>\</ul> : block
#### \<li>\</li> : block
<ul>
	<li >순서가</li>
	<li>없는</li>
	<li>리스트</li>
</ul>

```
<ul>
	<li>순서가</li>
	<li>없는</li>
	<li>리스트</li>
</ul>
```


### \<ol>\</ol> : block
#### \<li>\</li> : block
<ol> type??
	<li>순서가</li>
	<li>있는</li>
	<li>리스트</li>
</ol>

```
<ol>
	<li>순서가</li>
	<li>있는</li>
	<li>리스트</li>
</ol>
```


### \<dl>\</dl> : block
#### \<dt>\</dt> : block
#### \<dd>\</dd> : block


### <table></table> : block
#### <th></th>
#### <td></td>
#### <tr></tr>



### \<a>\</a> : inline
- 링크를 건다.
- href는 hypertext reference의 약자로 링크를 거는 타겟의 주소나 정보를 말한다.
- <a href="https://www.naver.com" target="_self">네이버로 이동</a> : target="_self"(기본) 삭제 가능 : 현재창에서 링크 이동.
- <a href="https://www.naver.com" target="_blank">네이버로 이동</a> : target="_blank" : 새창에서 링크 이동.
- <a href="#linkTest">Tags 메뉴로 이동</a> : href에 #과 해당 태그의 id값을 넣으면 그곳에 링크 이동.
- 다운로드 기능?

```
- <a href="https://www.naver.com">네이버로 이동</a> : target="_self"는 삭제 가능
- <a href="https://www.naver.com" target="_blank">네이버로 이동</a>
- <a href="https://www.naver.com" target="_blank">네이버로 이동</a> : target="_blank" : 새창에서 링크 이동.
- <a href="#linkTest">Tags 메뉴로 이동</a> : href에 #과 해당 태그의 id값을 넣으면 그곳에 링크 이동.
```


### \<img src="" alt=""> : inline
- 단일태그.
- <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/100px-HTML5_logo_and_wordmark.svg.png" alt="HTML5 logo and wordmark.svg"> : src는 source의 약자로 불러올 이미지의 경로를 기입한다.
- <img src="error" alt="HTML5 logo and wordmark.svg"> : alt는 이미지에 대한 설명이다. 호출에 실패시 alt 문구만 출력된다.
- <img width="50px" height="50px" title="툴팁" src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/100px-HTML5_logo_and_wordmark.svg.png" alt="HTML5 logo and wordmark.svg"> : width나 height 속성을 이용해서 크기 조정 가능, title 속성은 툴팁 기능을 활성화 한다.
- scrset???

```
- <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/100px-HTML5_logo_and_wordmark.svg.png" alt="HTML5 logo and wordmark.svg"> : src는 source의 약자로 불러올 이미지의 경로를 기입한다.
- <img src="error" alt="HTML5 logo and wordmark.svg"> : alt는 이미지 호출에 실패했을 경우 나타날 문구다.
- <img width="50px" height="50px" title="툴팁" src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/100px-HTML5_logo_and_wordmark.svg.png" alt="HTML5 logo and wordmark.svg"> : width나 height 속성을 이용해서 크기 조정 가능, title 속성은 툴팁 기능을 활성화 한다.
```


### \<video>\</video> : inline



### \<audio>\</audio> : inline



### \<iframe>\</iframe> : inline



### \<canvas>\</canvas> : inline



### \<template>\</template> : inline



### \<form>\</form> : block
#### \<input /> : inline
#### \<textarea>\</textarea> : inline
#### \<output>\</output> : inline
#### \<button>\</button> : inline
#### \<label>\</label> : inline
인풋 관련 정리 하자.
- 사용자의 입력을 받고 입력 받은 데이터를 서버로 전송하는 용도.
- <form>
	  <input type="text" placeholder="입력 요구사항" />
  </form>
- 라디오, 체크박스 사용? 
- 폼 테그에서 서버로 데이터를 보내는 방법?



### \<dialog>\</dialog> : block



### \<select>\</select> : inline
- 콤보박스? select list?


### \<datalist>\</datalist> : inline
- 콤보박스? selecte list?


<br>

## Tags : 의미론적 태그

### \<header>\</header> : block
- 제목


### \<nav>\</nav> : block
- 네비게이션


### \<aside>\</aside> : block


### \<section>\</section> : block


### \<main>\</main> : block


### \<footer>\</footer> : block
- 하단

### \<article>\</article> : block
- 본문

### \<details>\</details> : block


### \<thead>\</thead>


### \<tbody>\</tbody>


### \<tfoot>\</tfoot>



## Attribute
	모질라 보고 정리를 한번...

### class
	선택자, 중복 가능, 한 태그 안에 다수개 사용 가능.

### id
	선택자, 중복 불가, 한 태그 안에 하나만 가능.

### type

### style

### maxlength

### scope

### colspan

### rowspan

### data-
	사용자 정의 속성처럼 사용할 수 있다.
	'data-' 뒤로 어떤 속성이든 붙여서 사용할 수 있다.

### lang

## Event

### oninput