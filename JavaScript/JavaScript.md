# JavaScript
> 출처 : [developer.mozilla.org](https://developer.mozilla.org/ko/docs/Web/JavaScript)


## 변수 / 상수
> 변수명 선언 규칙.
>	- 변수명에는 문자, 숫자, $, _ 만 사용 가능.
>	- 첫 글자는 숫자가 올 수 없음.
>	- 기본 예약어는 사용 불가능.
>	- 상수에는 대문자로만 사용하여 상수임을 확인 시켜주는 것을 권장한다.
>	- 읽기 쉽고 이해하기 쉬운 표현식 사용을 권장한다.
>
> 변수는 let, 상수는 const 를 사용해서 선언한다.
>	- var를 사용하거나 생략 가능하지만 중복 선언 등의 문제로 추천하지 않는다.

```javascript
const NAME = "hoofac";	// 상수
let age = 38			// 변수
```

## 자료형
### 기본자료형
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
> 값이 할당되지 않았을 경우 나타난다.
	
	```javascript
	let age;
	undefined
	```

- symbol


### Reference
> object


### typeof 연산자
> 변수의 자료형을 확인할 때 사용한다.


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

## Location
> URL 주소를 가져온다.

- Location.href
	- 온전한 URL을 가져온다.

	```
	Location.href
	```

- Location.origin
	- 메인 URL 주소를 가져온다.

	```
	Location.origin
	```

- Location.pathname
	- 메인 주소 뒤('/') 이후의 경로 주소를 가져온다.

	```
	Location.pathname
	```

- Location.search
	- URL '?' 이후의 쿼리스트링을 가져온다.

	```
	Location.search
	```
