## map() 이란 무엇인가?
> map()은 배열의 메서드로 존재하며, 배열의 모든 요소에 함수를 적용한 새로운 배열을 반환한다.

### 자바스크립트에서 map()을 사용하는 상황
+ 배열의 각 값을 변형하고 싶을 때
+ HTML 요소를 동적으로 만들 때 (리액트 등에서도 자주 사용)

#### javascript
```
array.map(function(element, index, array) {
  // return 변환할 값
})

```
+ element: 배열 요소 하나
+ index (선택): 해당 요소의 인덱스
+ array (선택): 원본 배열 전체

### 간단한 코드 예제 
```
const numbers = [1, 2, 3, 4, 5];
const squared = numbers.map(function(x) {
  return x * x;
});

console.log(squared);  // [1, 4, 9, 16, 25]

```
