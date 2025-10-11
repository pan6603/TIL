## TypeScript 배열
> TypeScript에서 배열(Array) 은 “같은 종류의 데이터 여러 개를 한 변수에 담을 수 있는 자료 구조”이다.
쉽게 말해서, 많은 데이터를 하나의 이름으로 관리할 수 있게 해주는 ‘상자 모음’이다.

### 기본 배열 선언
```
// 숫자 배열
let numbers: number[] = [1, 2, 3, 4, 5];

// 문자열 배열
let fruits: string[] = ["apple", "banana", "cherry"];

// 불리언 배열
let flags: boolean[] = [true, false, true];

```

### 제네릭(Generic) 문법으로 배열 선언
```
let names: Array<string> = ["Alice", "Bob", "Charlie"];
let scores: Array<number> = [90, 85, 70];

```

### 객체 배열
```
type Student = {
  id: number;
  name: string;
  score: number;
};

let students: Student[] = [
  { id: 1, name: "Alice", score: 90 },
  { id: 2, name: "Bob", score: 80 },
  { id: 3, name: "Charlie", score: 85 },
];

```

### 배열 메서드 사용

```
let numbers: number[] = [10, 20, 30, 40];

// forEach
numbers.forEach(num => console.log(num));

// map
let doubled = numbers.map(num => num * 2);  // [20, 40, 60, 80]

// filter
let filtered = numbers.filter(num => num > 20);  // [30, 40]

// find
let found = numbers.find(num => num === 30); // 30

// push / pop
numbers.push(50);
numbers.pop();
```


### 유니언 타입 배열
```
let mixed: (string | number)[] = ["apple", 10, "banana", 20];

```



