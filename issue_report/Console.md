>참고 : [많이 뜨는 에러 10가지](https://blog.meeta.io/10)

함수 수정시 : 함수 내용만 수정했을때, 브라우저 캐시 상에서는 내부까지 체크를 안하니까 변경사항이 적용되지 않을 수도 있다.

## Uncaught SyntaxError
```
Uncaught SyntaxError: Identifier 'kim' has already been declared
```
- 변수를 재 할당하려 시도하면 나타난다.
- let, const는 재 할당을 허용하지 않는다.
- var을 이용하면 해결 가능하지만 추천하지 않는다.
- 변수명을 수정해서 할당 문제를 해결할 것을 추천한다.

```
Uncaught TypeError: Cannot read properties of undefined (reading '속성명')
```
- 속성을 읽을 수 없는 상황이다.
- 할당(=)을 이상한 기호(:, .) 등으로 잘못 입력했거나 속성의 대상, 혹은 대상에 속성이 존재하지 않을때 나타날 수 있다.

## Uncaught TypeError: [{(intermediate value)}] is not a function
- 즉시실행함수의 실행에 문제 발생.
- 윗줄의 무언가와 내용이 합쳐지며 발생.
- 해결 : 윗줄에 ; 넣어주면 Clear

## Uncaught TypeError: Assignment to constant variable
- const(상수) 선언되어 있는 변수에 값을 변경하려할 때 나타난다.