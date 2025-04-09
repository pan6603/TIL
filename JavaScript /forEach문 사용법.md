## forEach문 이란? 
> forEach문은 JavaScript에서 배열(Array)에 있는 각 요소를 순서대로 하나씩 꺼내어 어떤 작업을 수행할 때 사용하는 반복문이다.

### 예시 
```
배열.forEach(function(요소, 인덱스, 배열) {
  // 실행할 코드
});

```


```
let fruits = ['apple', 'banana', 'cherry'];

fruits.forEach(function(fruit, index) {
  console.log(index + ': ' + fruit);
});

```

### 정리 
+ forEach는 배열의 길이만큼 자동 반복.
+ 배열의 각 요소를 순서대로 꺼내서 함수에 전달.
+ 기존 for문보다 간결하고 가독성이 좋다.
+ break나 return으로 반복문을 중단할 수 없다.
