# 8. for문

## 8.1. for문

- 특정 코드를 반복해서 실행 for, while, do while

```txt
for(초기값; 조건식; 증감;) {
  문장;
  ...
}
```

```js
// for의 조건식이 참인 동안 문장들을 반복 실행
// 1. i의 값을 1로 초기화
// 2. 조건식 1 <= 3 참, 1 출력
// 3. i의 값이 1 증가
// 4. i의 값이 2가 됨
// 5. 조건식 2 <= 3 참, 2 출력
// 6. i의 값이 1 증가
// 7. i의 값이 3가 됨
// 8. 조건식 3 <= 3 참, 3 출력
// 9. i의 값이 1 증가
// 10. i의 값이 4가 됨
// 11. 조건식 4 <= 3 거짓, for 루프를 빠져나감

// 조건식 해석 : i가 3이하인 "동안에" 동작
for (let i = 1; i <= 3; i++) {
  console.log(i);
}

//  for 문을 이용해서 1 ~ 100 정수의 합계를 구하는 프로그램
let sum = 0;

// i가 1에서 100까지 값을 가지는 동안
for (let i = 1; i <= 100; i++) {
  // 문장이 반복 실행되며, 변수 sum에 1 ~ 100의 누적 합계를 저장
  sum += i;
}

// sum의 값을 출력
console.log(sum);

// for문, 배열, 템플릿 문자열(``)을 이용하여 웹페이지 글자에 색을 설정
const color = ["red", "green", "blue", "pink"];
let text = "";

// i는 0, 1, 2, 3의 값을 가지는 동안
for (let i = 0; i <= 3; i++) {
  // 템플릿 문자열을 이용
  text += `<span style="color:${color[i]}">안녕</span>`;
}

console.log(text);
document.write(text);
```

## 8.2. for in 문

- 객체의 요소들을 반복해서 읽어올 때 for in

```js
const member = { id: "kdhong", username: "홍길동", age: 30 };

// 객체의 요소 수 만큼, 즉 세번 반복 루프 진행
for (let x in member) {
  console.log(member[x]);
}
```

## 8.3. for of 문

```txt
for(변수 of 배열){
  문장;
  ...
}
```

```js
const scores = [88, 75, 95, 90, 78];

for (let score of scores) {
  console.log(score);
}
```
