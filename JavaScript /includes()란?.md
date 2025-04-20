## includes()란?
> includes()는 문자열 또는 배열 안에 특정 값이 포함되어 있는지 확인할 때 사용하는 메서드이다.

### 1. 문자열에서 사용

#### 문법
```
string.includes(searchString, position)

```
+ searchString: 찾고 싶은 문자열
+ position (선택): 검색을 시작할 인덱스 (기본값은 0)

#### 코드 예제
```
let text = "Hello, world!";
console.log(text.includes("world"));  // true
console.log(text.includes("World"));  // false (대소문자 구분)

```

### 2. 배열에서 사용
```
array.includes(searchElement, fromIndex)

```
+ searchElement: 배열에서 찾고 싶은 요소
+ fromIndex (선택): 검색 시작 위치 (기본값은 0)

#### 코드 예제 
```
let fruits = ["apple", "banana", "mango"];

console.log(fruits.includes("banana"));  // true
console.log(fruits.includes("grape"));   // false

```


