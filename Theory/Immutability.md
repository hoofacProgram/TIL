# Immutability : 불변성

# Mutability : 가변성

## Nested object
- 객체 안에 속성 중에 객체가 존재하는 경우, 중첩 객체(Nested object)라고 한다.

<br/>
<br/>

### const vs Object.freeze()
- const는 변수에 할당 값을 수정할 수 없도록 하는 기능을 수행한다.
- Object.freeze()는 할당 값에 연결된 데이터를 수정할 수 없도록 막는 기능을 수행한다.
- const는 변수 할당 값의 수정을 시도할 경우 console에 error를 출력한다.
- Object.freeze()는 error 없이 기능 수행만 막는다.