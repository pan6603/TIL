## reverse() 메서드는 무엇인가?
> reverse() 메서드는 JavaScript에서 배열의 요소 순서를 반대로 뒤집는 메서드입니다. 원본 배열을 직접 변경하며, 변경된 배열을 반환합니다.

### 코드 예제 

1. 원본 배열을 뒤집기

```
let arr = [1, 2, 3, 4, 5];
let reversedArr = arr.reverse();

console.log(reversedArr);
console.log(arr);
```

2. 원본을 유지하는 방법

```
let arr = [1, 2, 3, 4, 5];
let reversedArr = [...arr].reverse();

console.log(reversedArr);
console.log(arr);
```

3. 문자열을 뒤집기

```
let str = "hello"
let result = str.split("").reverse().join("");

console.log(result);
```









