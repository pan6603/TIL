## join() 배열 메서드
> join()은 JavaScript 배열(Array)의 메서드 중 하나로, 배열의 요소들을 하나의 문자열로 합쳐준다.

### 사용이유 
join()을 사용하는 이유는 배열을 문자열로 쉽게 변환하고, 그 과정에서 원하는 구분자(separator)를 삽입할 수 있기 때문이다.

### 문법
```
array.join(separator)
```
+ separator (구분자): 선택 사항. 요소 사이에 넣을 문자열을 지정한다.

### 기본 사용 
```
const fruits = ['사과', '바나나', '포도'];
const result = fruits.join();  
console.log(result);  // "사과,바나나,포도"

```

### 구분자 지정
```
const fruits = ['사과', '바나나', '포도'];
const result = fruits.join(' / ');
console.log(result);  // "사과 / 바나나 / 포도"

```

### 문자열 split() → join()으로 변환하기
```
const sentence = "안녕하세요 자바스크립트!";
const result = sentence.split(' ').join('-');
console.log(result);  // "안녕하세요-자바스크립트!"

```


