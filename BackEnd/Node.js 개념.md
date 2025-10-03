## Node.js 무엇이나요? 
> Node.js는 자바스크립트를 브라우저 밖, 서버 환경에서도 실행할 수 있게 만든 실행 환경(Runtime Environment) 이다.

### 배경
+ 원래 자바스크립트는 **웹 브라우저 안에서만** 돌아간다. (버튼 클릭, 화면 변화 같은 프론트엔드 용도)
+ 그런데 **구글의 V8 엔진**을 기반으로 만들어진 Node.js 덕분에,
  이제는 **브라우저 밖에서도 자바스크립트를 실행**할 수 있게 되어있다.


### Node.js 특징

1. **이벤트 기반(비동기 처리)**

   * 동시에 많은 요청을 빠르게 처리 가능 → 실시간 서비스(채팅, 스트리밍)에 강함.

2. **단일 스레드**

   * 한 개의 스레드로 동작하지만, 이벤트 루프를 사용해서 여러 작업을 효율적으로 처리.

3. **NPM (Node Package Manager)**

   * 오픈소스 라이브러리를 쉽게 설치해서 사용 가능. (`express`, `mongoose`, `axios` 등)

4. **빠른 속도**

   * 구글 V8 엔진 덕분에 자바스크립트 실행 속도가 빠름.

---

### Node.js 서버 예제

```javascript
// Node.js 내장 모듈 불러오기
const http = require("http");

// 서버 만들기
const server = http.createServer((req, res) => {
  res.writeHead(200, { "Content-Type": "text/plain" });
  res.end("Hello Node.js!");
});

// 서버 실행
server.listen(3000, () => {
  console.log("서버 실행 중: http://localhost:3000");
});
```


---

### 📌 정리

* **Node.js = 자바스크립트 실행 환경**
* 브라우저 밖에서도 자바스크립트 실행 가능
* 프론트엔드뿐만 아니라 **백엔드 서버 개발**까지 자바스크립트로 가능

---


