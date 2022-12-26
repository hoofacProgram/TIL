# JavaScript
> [developer.mozilla.org](https://developer.mozilla.org/ko/docs/Web/JavaScript)


## 변수 / 상수
	변수명 선언 규칙.
	- 변수명에는 문자, 숫자, $, _ 만 사용 가능.
	- 첫 글자는 숫자가 올 수 없음.
	- 기본 예약어는 사용 불가능.
	- 상수에는 대문자로만 사용하여 상수임을 확인 시켜주는 것을 권장한다.
	- 읽기 쉽고 이해하기 쉬운 표현식 사용을 권장한다.
	- 변수는 let, 상수는 const 를 사용해서 선언한다.
	- const를 default로 사용하고, 필요시 let를 사용한다.
	- var를 사용하거나 생략 가능하지만 중복 선언 등의 문제로 추천하지 않는다.
	- const [] = [] 와 같은 방식으로 다중 선언이 가능하다.

```javascript
const NAME = 'hoofac'	// 상수
let age = 38			// 변수
const [NAME, AGE] = ['hoofac', 38]
```

## 자료형
### primitive : 기본자료형
	데이터 불변성.
	메모리를 직접 할당받아 사용한다.
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
	- false를 가지는 경우의 수.
	```javascript
	// 기본형
	undefined
	null
	NaN
	0(-0)
	''	// 빈 문자열은 false, 빈 배열([])과 빈 객체({})는 true
	false
	NaN === NaN	// null === null, undefined === undefined는 true
	```
	
- Null
	- 존재하지 않는 값.
	
	```javascript
	let money = null;
	null
	```

- Undefined

	값이 할당되지 않았을 경우 나타난다.
	
	```javascript
	let age;
	undefined
	```

- Symbol




### Reference : 참조자료형 : 객체
	데이터 가변성.
	모든 참조자료형은 그 자체로 객체다.
	임의의 메모리에 값을 넣고, 그 주소값을 할당받아 사용한다.
- Object
	- Object.assign({}, 변수명1, 변수명2)
		- 첫번째 {} 인자에 두번째 이후의 인자 내용들을 합쳐서 넣어준다.
		- 변수 인자를 하나만 넣으면 복사처럼 사용된다.
	```javascript
	function setName(man) {
		// Object.assign으로 인해 lim의 데이터는 kim의 데이터와 개별적으로 구분되었다.
		man = Object.assign({}, man)
		man.name = 'lim'
		return man
	}

	- Object.freeze(변수명)
		- 변수를 수정할 수 없는 상태로 만들어준다.
		- 함수를 실행하면 풀 수 있는 방법이 존재하지 않는다.
		- 수정이 필요할 시, 복제를 통해 새로운 변수로 만들어 사용한다.
		- Nested object의 경우에는 변경이 가능하다.
	const kimN = {name: 'kim'}
	const limN = setName(kimN)
	```
- Array
	- array.concat()
	- [] 복사시, .concat()을 해줌으로 중복 nested object 현상으로 인한 값 공유 현상을 해결할 수 있다.
	```javascript
	// concat 사용하는 예제 만들어서 넣어놓자!
	```
- Function
- etc.

### typeof 연산자
> 변수의 자료형을 확인할 때 사용한다.


## 메시지창

## 형변환

## 기본 연산자

## 비교 연산자

Null 병합 할당자??

## 논리 연산자
- || : or
	- 앞과 뒤의 값 중 하나라도 true라면 true다.
	- 앞의 값이 true면 뒤에 값은 확인하지 않는다.
```javascript
// 함수 사용
if (false || true) {
	return true
}
// 변수 사용
let f = false
let t = '앞의 값이 false면 뒤의 값이 입력된다.'
const X = f || t
console.log(x)	// '앞의 값이 false면 뒤의 값이 입력된다.'
```

## 조건문

## 반복문

## swich문

## 함수
### 함수 표현식
### 화살표 함수
### IIFE(즉시 실행 함수 표현)
- ()() : 소괄호 두개
- 첫번째 () 괄호 안에 실행할 함수 등을 입력한다.
- 두번째 () 괄호는 비워둔다.
```javascript
(function () {
	
})()
```



## 객체

## Array
	const(상수) 선언해서 사용
```
const array = []
```
- array.push()
	- array가 가진 데이터에 직접적으로 접근해서 추가 데이터를 입력한다.
	```javascript
	```
- array.concat()
	- array가 가진 데이터를 복사하거나, 복사한 데이터에 추가 데이터를 입력할 경우 사용한다.
	- object 복사시, .concat()을 해줌으로 중복 nested object 현상으로 인한 값 공유 현상을 해결할 수 있다.
	- push()에 비해 성능이 떨어지므로, 필요시에만 사용을 권장한다.
	```javascript
	예제필요
	```
## 동기, 비동기
### Promise
#### then
```javascript
.then()
```
### Async / Await


## Console
- console.log()
```javascript
console.log('출력하고 싶은 내용')
```

## Location
> URL 주소를 가져온다.

### Location.href
	온전한 URL을 가져온다.
```
Location.href
```

### Location.origin
	메인 URL 주소를 가져온다.

```
Location.origin
```

### Location.pathname
	메인 주소 뒤('/') 이후의 경로 주소를 가져온다.

```
Location.pathname
```

### Location.search
	URL '?' 이후의 쿼리스트링을 가져온다.

```
Location.search
```
