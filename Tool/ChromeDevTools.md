# ChromeDevTools
## Console

## Sources

## Network
### Preview
- SpGetData : 내가 상대에 보내는 데이터 확인.
- SpSetData : 상대에게 내가 받는 데이터 확인.


## [Redux DevTools](https://github.com/reduxjs/redux-devtools)
- Redux를 이용한 상태 변경 히스토리를 확인, export, import 등... 디버깅에 탁월한 기능을 제공한다.
- 설치 및 사용설정
    - [설치 관련 정보](https://github.com/reduxjs/redux-devtools/tree/main/extension#installation) 링크를 참고해서 설치한다.
    - store 생성시 'window.__REDUX_DEVTOOLS_EXTENSION__ && window.__REDUX_DEVTOOLS_EXTENSION__()' 를 추가해준다.
```javascript
    const store = Redux.createStore(
      reducer
      , window.__REDUX_DEVTOOLS_EXTENSION__ && window.__REDUX_DEVTOOLS_EXTENSION__()  // Redex DevTools 사용을 위한 추가
      )
```

## 추가 예정...
- console 보고 에러 내용 확인하자
- watch에서 한줄씩 명령으로 실행 시켜볼 수 있다
