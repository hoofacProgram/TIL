# jQuery
>출처 : [jquery API](https://api.jquery.com)

## Selector
- $()
- lt() : 작은것
- gt() : 큰것
- .eq() : 같은 것
- .css() : style 속성 설정


- val()
- prop()
- attr()


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