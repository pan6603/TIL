## setTimeOut이란 무엇인가?
> 자바스크립트에서 setTimeout은 특정 시간이 지난 후에 함수를 한 번 실행하게 해주는 함수이다.

### 사용하는 이유
일정 시간 후에 어떤 동작을 실행하고 싶을 때 사용. 

### 기본문법 

#### javascript
```
setTimeout(function, delay);
```
+ function: 나중에 실행될 함수
+ delay: 몇 밀리초(ms) 후에 실행할지 정하는 숫자 (1초 = 1000ms)

### 코드예제 

```
console.log("1초 후에 메시지를 보여줍니다!");

setTimeout(function() {
  console.log("안녕하세요! 1초 지났어요.");
}, 1000);

```
+ setTimeout은 1초(=1000ms) 후에 console.log 출력이 된다.

### 화살표 함수 
```
setTimeout(() => {
  console.log("2초 후 실행!");
}, 2000);

```

### 정리 
+ setTimeout은 한 번만 실행된다.


