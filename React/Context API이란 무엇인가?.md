## Context API이란 무엇인가?
> Context API란 주로 React(리액트)에서 사용되는 기능으로, 컴포넌트들 사이에서 데이터를 쉽게 공유할 수 있게 해주는 API이다.

### 쉬운 설명
+ 일반적으로 리액트에서는 부모 컴포넌트에서 자식 컴포넌트로만 데이터를 전달할 수 있습니다(Props 사용).
+ 하지만 컴포넌트가 여러 단계로 깊어지면, 중간에 필요 없는 컴포넌트까지 계속 데이터를 전달해야 해서 불편합니다.
+ Context API를 사용하면, 이런 번거로움 없이 ‘전역 상태’처럼 데이터를 여러 컴포넌트에서 쉽게 꺼내 쓸 수 있습니다.

### 주요 특징
+ 전역 데이터 저장소 역할
+ 여러 단계의 컴포넌트가 있어도, 원하는 곳에서 바로 데이터 접근 가능
+ 주로 테마(Theme), 사용자 정보(User), 언어(Language) 등 앱 전체에서 자주 쓰는 값을 저장할 때 사용

### 간단한 사용 코드 
```
import React, { createContext, useContext } from 'react';

// 1. Context 생성
const MyContext = createContext();

function App() {
  return (
    // 2. Provider로 값 전달
    <MyContext.Provider value={"Hello Context"}>
      <Child />
    </MyContext.Provider>
  );
}

function Child() {
  // 3. useContext로 값 꺼내서 사용
  const value = useContext(MyContext);
  return <div>{value}</div>;
}
```

### 정리 
Context API는 리액트에서 여러 컴포넌트가 데이터(상태)를 쉽게 공유할 수 있게 해주는 기능이다.
