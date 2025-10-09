## Express 개념
> Node.js 환경에서 서버를 쉽게 만들 수 있게 도와주는 웹 프레임워크, Express = Node.js로 서버를 더 간편하게 만드는 도구이다.

### 1. 서버 구축이 훨씬 쉬워짐

```
// Express 예시
const express = require('express');
const app = express();

app.get('/', (req, res) => {
  res.send('Hello Express!');
});

app.listen(3000, () => console.log('서버 실행 중'));

```
+ Node.js만으로 HTTP 서버를 만들려면 코드가 꽤 복잡하다.
+ 하지만 Express를 쓰면 몇 줄만으로 서버를 실행할 수 있다.


### 2. Node.js 기본 모듈(http)로 하면
```
const http = require('http');

const server = http.createServer((req, res) => {
  if (req.url === '/') {
    res.write('Hello Node!');
    res.end();
  }
});

server.listen(3000);

```

### 3. 미들웨어(Middleware) 시스템
Express의 가장 강력한 기능 중 하나이다. 요청(Request)이 들어올 때, 중간에서 여러 단계의 처리를 쉽게 넣을 수 있다. 

### 예를 들어:
+ 로그 출력
+ 사용자 인증
+ 요청 본문 파싱
+ 에러 처리

```
app.use(express.json()); // JSON 데이터 파싱
app.use((req, res, next) => {
  console.log(req.method, req.url);
  next();
});

```


### 4. 라우팅 관리가 쉬움
```
app.get('/users', (req, res) => res.send('유저 목록'));
app.post('/login', (req, res) => res.send('로그인 처리'));

```

### 5. 가볍고 유연함
Express는 “필요한 기능만 추가하는” 구조라서, NestJS나 Django처럼 무겁지 않고 빠르게 개발할 수 있다.










