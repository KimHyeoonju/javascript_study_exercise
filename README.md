# 3. 데이터형(Data Type)

- number : 숫자
- string : 문자
- boolean : true, false
- null
- undefined
- Bigint
- object : 객체
- symbol

## 3.1. 숫자 number

```js
const a = 3; //정수(integer)
const b = 5.7; // 부동 소수점 숫자 (floating point number)
const c = 123e3; // 123000
const d = 123e-3; // 0.123

console.log(a);
console.log(b);
console.log(c);
console.log(d);
```

## 3.2. Bigint

- 정수는 15개의 숫자, 15자리 숫자까지 나타낼 수 있다.
- 그 이상의 정수를 사용하려면 Bigint 형을 사용해야 한다.

```js
const e = 123456789123456789;
const f = 123456789123456789n;

console.log(e);
console.log(f);
```

## 3.3. 문자열 string

```js
// , 는 자동 한칸 띄움, + 는 띄우기 없음.

// 문자열
const text1 = "사 과"; // 큰 따움표 사용
console.log("text1에 저장된 내용 : ", text1);

// length : 문자열 길이
// 문자열의 length 프로퍼티(속성) 사용, 공백도 포함
console.log("text1의 문자열 길이는 " + text1.length + "입니다.");

// 템플릿 문자열 ``
// 이 나오면서 위와 같이 쓸 필요 없어졌다.
let username = "홍길동";
let age = 30;
let text2 = "이름 : " + username + "나이는 : " + age;
console.log(text2);

let text3 = `이름 : ${username}, 나이는 : ${age}`;
console.log(text3);
```

## 3.4. boolean

```js
let x = 5 > 3; // true
let y = 5 < 3; // false

console.log(x, y);
```

## 3.5. undefined, null(빈 문자열)

```js
let x;
let y = "";

console.log(x);
// typeof : 변수 타입 출력
console.log(typeof y);
```

## 3.6. 객체 object

```js
const member = {
  id: "kdhong",
  name: "홍길동",
  age: 20,
};

console.log(member);
console.log("아이디 :", member.id);
console.log(member.age);
console.log(member.name);
```

## 3.7. 심볼 symbol

- number, string, boolean 과 같은 원시데이터
- 유일한 식별자로서 객체의 속성을 추가하는데 사용
