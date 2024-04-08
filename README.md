# 2. 변수

- 데이터가 컴퓨터 메모리에 저장되는 주소

# 2.1. 변수 선언

- 변수 선언 키워드 : var, let, const
- var : 전역 변수, 다른 파일에서도 접근이 가능하기 때문에 var 사용 비추천
- const : 재할당 불가
- let : 재할당 가능
- const 주로 사용 이 외의 경우는 let으로 사용.

```js
let keyword = "키워드 let으로 변수 name을 선언했다.";
console.log(keyword);

// 필요에 따라 값을 재할당 할 수 있다.
keyword = "변수 name에 홀길동 저장";
console.log(keyword);
```

## 2.2. 변수 이름 짓기

- 변수 이름에는 영어, 숫자, 밑줄, $ 사용가능
- **주의! 숫자로 시작하면 안됨**
- 대소문자 구분
- 일반적으로 카멜케이스 사용

```js
const a = 5;
const font1 = "돋움";
const _price = 30000;
const maxWidth = 600;
const max_width = 800;
```
