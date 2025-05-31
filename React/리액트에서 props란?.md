## 리액트에서 props란?
> 리액트(React)에서 props는 컴포넌트 간에 데이터를 전달할 때 사용하는 객체이다. 부모 컴포넌트가 자식 컴포넌트에게 값을 넘겨줄 때 사용한다.

### ✅ 특징
+ props는 'properties(속성)'의 줄임말
+ 부모 → 자식 컴포넌트로 데이터를 전달하는 통로
+ 자식 컴포넌트는 전달받은 값을 읽기만 할 수 있음 (수정은 불가능)

✅ 코드 예시
```
// 부모 컴포넌트
function App() {
  return <Greeting name="길동" />;
}

// 자식 컴포넌트
function Greeting(props) {
  return <h1>안녕하세요, {props.name}님!</h1>;
}

```
📌 여기서:

+ App이 부모 컴포넌트
+ Greeting이 자식 컴포넌트
+ 부모가 name="길동" 이라는 데이터를 props로 전달함
+ 자식은 props.name 으로 받아서 화면에 출력

### ✅ 자주 사용하는 패턴
구조 분해 할당으로 props 받기:
```
function Greeting({ name }) {
  return <h1>안녕하세요, {name}님!</h1>;
}

```

### ✅ props 특징 정리
+ 단방향 데이터 흐름	부모 → 자식 방향으로만 전달됨
+ 읽기 전용	자식 컴포넌트는 props를 변경할 수 없음
+ 재사용성 증가	다양한 데이터를 props로 받아 다양한 형태로 렌더링 가능

