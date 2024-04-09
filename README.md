# 4. 연산자

- 산술연산자
- 할당연산자
- 비교연산자
- 논리연산자

## 4.1. 산술연산자

```txt
+
-
*
/ : 나누기 - 값
% : 나누기 - 나머지
** : 거듭제곱
++ : 1 증가
-- : 1 감소
```

## 4.2. 할당연산자

- 할당(assign) 연산자는 데이터나 변수 값을 변수에 저장. 즉, 메모리 공간에 할당하는 역할

```js
let a = 10,
  b = 20,
  c = 30,
  d = 40,
  e = 50;
```

```js
let username = "홍길동";
let tel = "010-1234-5678";
let age = 30;

let text = "";

text += "<table border=1>";

text += "<tr><th>이름</th><th>전화번호</th><th>나이</th></tr>";

text +=
  "<tr><td>" + username + "</td><td>" + tel + "</td><td>" + age + "</td></tr>";

text += "</table>";

document.write(text);
```

## 4.3. 비교연산자

```js
let a = 3,
  b = "3",
  c = 5,
  d = 3;

console.log(a == b); // true
console.log(a === b); //false
console.log(a != b); //false
console.log(a !== b); // true
console.log(a > c); //false
console.log(a < c); // true
console.log(a >= c); //false
console.log(a <= c); // true
```

## 4.4. 논리연산자

- && : AND 두 조건이 모두 true 일 경우에만 true 를 반환
- || : OR 두 조건 중 하나이상 true 일 경우 true 를 반환
- ! : NOT 결과가 true 인 경우 false 를 반환, 반대로 false 인 경우 true 를 반환
