# jQuery
>[jquery API](https://api.jquery.com)

## Selector
- $()
- $('#id') : id
- $('.class') : class
- $('tag') : tag
- $('[attr]') : attribute
- $('#parent > div') : id가 parent인 요소의 div 속성을 가진 자식 / 구분자 : >
- $('#parent div') : id가 parent인 요소의 div 속성을 가진 후손 / 구분자 : 공백

```javascript
$('#id')
$('.class')
$('tag')
$('[attr]')
$('#parent > div')
$('#parent div')
```

## Attribute
### attr()
- 태그에 속성을 추가한다.
```javascript
$('h1').attr('disabled', true)
// <h1 disabled = "true"></h1>
```

### text()
- 요소의 텍스트를 가져오거나 변경할 때 사용한다.
```javascript
$('h1').text()  // 텍스트를 가져온다.
$('h1').text('텍스트')  // 텍스트를 입력한다.
```

### disabled
- 비활성화

### select 요소에 option 추가 하는방법?

### val()
### prop()
### attr()

### lt() : 작은것
### gt() : 큰것
### eq() : 같은 것
### css() : style 속성 설정
### find() : 선택자의 하위 요소 중 해당 요소를 찾는다.


## Event

### $(document).ready()
    DOM 생성 완료시 호출된다.
    두가지 형태로 사용 가능하다.
```javascript
$(function () {
  // 최신 버전
})
```
```javascript
$(document).ready(function () {
  // 1.8 버전 이후에는 사용되지 않는다.
})
```

### $(window).resize()
    윈도우의 크기가 바뀔 때 실행된다.

### data()
- 태그에 data-(사용자 정의) 속성을 추가한다.
```javascript
$('h1').data('foo', 20)
// <h1 data-foo="20"></h1>
$('h1').data('foo', {age:20, name:'Lee'})
// <h1 data-foo='{"age":"20", "name":"Lee"}'></h1>
```

### trigger()


### onclick()
- click 이벤트 추가
- 함수식으로 넣으면 안에 파라미터 전달도 가능
```javascript
$('#home').on('click', () => { 함수명(파라미터)} );
```

### change()
- 요소에 change 이벤트 추가
```javascript
$('#nm').change(() => {
  // 실행할 내용
})
```


- fadeIn
- fadeOut
- fadeTo

