# JavaScript
>출처 : [youtube/코딩앙마/자바스크립트 기초 강좌](https://www.youtube.com/playlist?list=PLZKTXPmaJk8JDicsOyY2cTcwXmBa-ZceI)


## 변수 / 상수
- 변수명 선언 규칙.
	- 변수명에는 문자, 숫자, $, _ 만 사용 가능.
	- 첫글자는 숫자가 올 수 없음.
	- 기본 예약어는 사용 불가능.
	- 가급적으로 상수는 대문자를 이용하여 상수임을 확인.
	- 읽기 쉽고 이해할 수 있는 표현식 사용.
- let(변수), const(상수)를 사용해서 선언.
	- var를 사용하거나 생략 가능하지만 중복 선언 등의 문제로 추천하지 않음.

```javascript
const NAME = "hoofac";
let age = 38 
```


## 자료형

### Primitive
- String
	- "String" (쌍따옴표), 'String' (홑따옴표), \`String` (백틱)
	
	```javascript
	const NAME_SINGLE = 'hoohac'
	const NAME_DOUBLE = "hoofac"
	const NAME_BACKTICK = `my name is ${NAME_DOUBLE}`
	```

	- 따옴표는 사용성에 차이 없음.
	- 따옴표 출력이 필요할 때는 \ 를 사용하여 표현 가능.
	- 백틱은 ${}를 이용하여 문자열 내부에 변수 표현 가능.
	
- Number
	- 정수, 실수 등, 숫자 모두 사용 가능.
	- 사칙연산(+, -, *, /, %) 가능.
	- 숫자를 0으로 나누면 Infinity(무한대).
	- 문자열을 숫자로 나누면 NaN(Not a Namber).

- Boolean
	- true(참), false(거짓)
	- 논리 연산 등에서 주로 사용.
	
- null
	- 존재하지 않는 값.
	
	```javascript
	let money = null;
	null
	```

- undefined
	- 값이 할당되지 않았을 경우.
	
	```javascript
	let age;
	undefined
	```

- symbol


### Reference
- object


### typeof 연산자
- 변수의 자료형을 확인할 때 사용.


## 메시지창

## 형변환

## 기본 연산자

## 비교 연산자

## 조건문

## 논리 연산자

## 반복문

## swich문

## 함수
### 함수 표현식
### 화살표 함수

## 객체

## 배열