# HTML
>출처 : [developer.mozilla.org](https://developer.mozilla.org/ko/docs/Web/HTML)
https://developer.mozilla.org/ko/docs/Learn/Getting_started_with_the_web/HTML_basics
https://developer.mozilla.org/ko/docs/Learn/HTML/Introduction_to_HTML/Getting_started


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


## Tags

### \<!DOCTYPE html>
- DOCTYPE은 HTML이 지켜야할 규칙에 대한 연결부? 같은 역할을 했다.
- 현재는 단지, 올바른 구동을 위한 규칙과 같은 선언으로 쓰인다.


### \<html>\</html>
- 전체 페이지를 감싸는 root 역할의 요소.


### \<head>\<head/>
- 페이지에 포함되어 있는 모든 숨겨진 내용들을 담고 있는 컨테이너.
- CSS, 문자 집합의 선언, 페이지에 대한 설명, 검색에 노출될 키워드 등... 페이지에 대한 모든 내용을 가진다.


### \<body>\</body>
- 

### \<h1>\</h1> ~ \<h6>\</h6>
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


### \<p>\</p>
- <p>문단</p><p>나누기</p>

```
- <p>문단</p><p>나누기</p>
```

### \<br/>
- 줄<br/>바꿈

```
- 줄<br/>바꿈
```


### \<b>\</b>
- bold, 텍스트를 <b>굵게</b> 표시.
- 중요 X, 일반 텍스트와 표시만 다를 뿐 <b>동일</b>하게 취급.

```
- bold, 텍스트를 <b>굵게</b> 표시.
- 중요 X, 일반 텍스트와 표시만 다를 뿐 <b>동일</b>하게 취급.
```


### \<strong>\</strong>
- 텍스트를 <strong>굵게</strong> 표시.
- 일반 텍스트에 비해 해당 content의 <strong>중요함</strong>을 알리는 용도 포함.

```
- 텍스트를 <strong>굵게</strong> 표시.
- 일반 텍스트에 비해 해당 content의 <strong>중요함</strong>을 알리는 용도 포함.
```

### \<i>\</i>
- italic, 텍스트를 <i>기울어지게</i> 표시.
- 중요 X, 일반 텍스트와 표시만 다를 뿐 <i>동일</i>하게 취급.

```
- italic, 텍스트를 <i>기울어지게</i> 표시.
- 중요 X, 일반 텍스트와 표시만 다를 뿐 <i>동일</i>하게 취급.
```


### \<em>\</em>
- italic, 텍스트를 <em>기울어지게</em> 표시.
- 일반 텍스트에 비해 해당 content의 <em>중요함</em>을 알리는 용도 포함.

```
- italic, 텍스트를 <em>기울어지게</em> 표시.
- 일반 텍스트에 비해 해당 content의 <em>중요함</em>을 알리는 용도 포함.
```

### \<ins>\</ins>
- <ins>밑줄</ins>을 표시.

```
- <ins>밑줄</ins>을 표시.
```
### \<del>\</del>
- 텍스트 중앙에 <del>취소선</del>을 표시.

```
- 텍스트 중앙에 <del>취소선</del>을 표시.
```

### \<q>\</q>
- <q>짧은 인용문에 사용.</q>

```
- <q>짧은 인용문에 사용한다.</q>
```


### \<blockquote>\</blockquote>
<blockquote>내용이 긴 인용문에 사용한다.</blockquote>

```
<blockquote>내용이 긴 인용문에 사용한다.</blockquote>
```

### \<ul>\</ul>
<ul>
	<li>순서가</li>
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


### \<ol>\</ol>
<ol>
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

### \<a>\</a>
- 링크를 건다.
- href는 hypertext reference의 약자로 링크를 거는 타겟의 주소나 정보를 말한다.
- <a href="https://www.naver.com">네이버로 이동</a>
- <a href="https://www.naver.com" target="_blank">네이버로 이동</a>

```
- <a href="https://www.naver.com">네이버로 이동</a>
```


