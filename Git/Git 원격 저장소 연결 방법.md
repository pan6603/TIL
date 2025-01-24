## Git 원격 저장소 연결 방법 
<p>Git 통해서 <strong>Github 원격 저장소와 연결</strong>하는 명령어 입니다. </p>

### 1. git init 프로젝트 초기화 하기 
```
git init 
```

### 2. github에서 만들었던 프로젝트 저장소 연결하기
```
git remote add origin http://example.com
```
git remote add origin 명령어를 통해서 뒤에 만들었던 저장소 주소 입력 <br>
그리고나서 git add . 명령어 입력


### 3. git commit
```
git commit -m "커밋 메세지 입력"
```

### 4. git push origin +main
```
git push origin +main
```
git push origin +main 명령어 입력 시 원격 저장소 연결 성공
