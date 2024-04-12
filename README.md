# 12. 생성자 함수와 클래스

## 12.1. 생성자 함수

### 12.1.1. 생성자 함수란?

- 생성자 함수(constructor function) 는 일반 함수와 기능적인 차이는 없다.
- 그러나 일반 함수와는 달리 생성자 함수는 new 연산자와 함께 자바스크립트에서 객체를 생성하기 위해 사용
- 생성자 함수를 정의할 때에는 일반함수와 구분하기 위해 첫 글자를 대문자로 시작

```js
// 생성자 함수의 객체 생성 예시

// 생성자 함수 Member 는 세 개의 매개변수 id, name, age 를 가진다.
function Member(id, name, age) {
  // 키워드 this 는 생성자 함수로 생성되는 객체 자신을 의미
  // 따라서 this.id 는 객체 자신의 프로퍼티 id를 의미
  this.id = id;
  this.name = name;
  this.aeg = age;
}

const member1 = new Member("kdhong", "홍길동", 30);
const member2 = new Member("kkim", "김길동", 40);
const member3 = new Member("gildong", "길동이", 12);

let text = "";
text += member1.name;
text += member2.name;
text += member3.name;

document.getElementById("show").innerHTML = text;
```

### 12.1.2. 생성자 함수의 메서드

```js
// 생성자 함수의 객체 생성 예시

// 생성자 함수 Member 는 세 개의 매개변수 id, name, age 를 가진다.
function Member(id, name, age) {
  // 키워드 this 는 생성자 함수로 생성되는 객체 자신을 의미
  // 따라서 this.id 는 객체 자신의 프로퍼티 id를 의미
  this.id = id;
  this.name = name;
  this.aeg = age;
  this.getName = function () {
    return `나의 이름은 ${this.name} 입니다.`;
  };
}

const member1 = new Member("kdhong", "홍길동", 30);
const member2 = new Member("kkim", "김길동", 40);
const member3 = new Member("gildong", "길동이", 12);

let text = "";
text += `${member1.name} <br>`;
text += `${member2.name} <br>`;
text += `${member3.name} <br>`;
text += `${member1.getName()}`;

document.getElementById("show").innerHTML = text;
```

## 12.2. 프로토타입

- 추후

## 12.3. 클래스

- 추후
