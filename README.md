# 13. 배열

## 13.1. 배열이란?

- 여러 값을 하나의 변수에 저장할 수 있게 해주는 특별한 변수 array

## 13.1.1. 배열의 생성

```js
const fruits = ["사과", "딸기", "참외"];

let text = "";
text += fruits;
text += fruits[0];
text += fruits[1];
text += fruits[2];

console.log(text);

const fruits1 = new Array("오렌지", "사과", "딸기", "참외");
console.log(fruits1);
```

## 13.1.2. 배열요소의 메서드들

### 13.1.2.1. join() 메서드

- join() 메서드는 배열을 문자열로 변환하는데 사용

```js
const animals = ["사자", "호랑이", "사슴", "펭귄"];

let str1 = animals.join();
let str2 = animals.join("/");

console.log(str1);
console.log(str2);
```

### 13.1.2.2. push() 메서드

- push() 메서드 : 배열의 끝에 새로운 요소를 추가하는데 사용

```js
const animals = ["사자", "호랑이", "사슴", "펭귄"];

let x = animals.push("도마뱀");

let text = "";
text += animals;

console.log(text);
```

### 13.1.2.3. pop() 메서드

- 배열의 마지막 요소를 삭제하는데 사용

```js
const animals = ["사자", "호랑이", "사슴", "펭귄"];

let x = animals.pop();

let text = "";
text += animals;

console.log(text);
```

### 13.1.2.4. shift() 메서드

- 배열의 첫 요소를 삭제

```js
const animals = ["사자", "호랑이", "사슴", "펭귄"];

let x = animals.shift();

let text = "";
text += animals;

console.log(text);
```

### 13.1.2.5. <span style="color:red"> splice() </span> 메서드

- 배열의 요소를 추가하거나 삭제할 때 사용

```js
const animals = ["사자", "호랑이", "사슴", "펭귄", "여우", "도마뱀"];

let text = "";
let arr = "";

// index 2인 요소 "사슴" 부터 3개의 요소를 삭제하고 "개구리" 삽입

arr = animals.splice(2, 3, "개구리");

console.log(animals);
console.log(arr);
```

### 13.1.2.6. <span style="color:red"> indexOf()</span> 메서드

- 배열에서 특정 문자열의 위치, 즉 인덱스 값을 반환

```js
const animals = ["사자", "호랑이", "사슴", "펭귄", "여우", "도마뱀"];

let index1 = animals.indexOf("사슴");

console.log(index1);
```

### 13.1.2.7. <span style="color:red">includes()</span> 메서드

- 특정 요소의 존재 여부를 파악

```js
const animals = ["사자", "호랑이", "사슴", "펭귄", "여우", "도마뱀"];

const result = animals.includes("악어");

console.log(result);
```

### 13.1.2.7. <span style="color:red"> slice() </span>메서드

- 인덱스를 이용하여 특정 요소를 추출

```js
const animals = ["사자", "호랑이", "사슴", "펭귄", "여우", "도마뱀"];

// 인텍스 1부터 인덱스 4 앞까지(4는 포함하지 않음)의 요소
const result = animals.slice(1, 4);

console.log(result);
```

### 13.1.2.7. <span style="color:red">find() </span>메서드

- 특정 요소를 찾는 조건을 콜백함수를 통해 전달하여 조건에 해당하는 첫 번째 요소 값을 반환
