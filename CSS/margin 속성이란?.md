## margin 속성이란?
> HTML과 CSS에서 margin은 요소의 바깥쪽 여백을 의미하며, 다른 요소와의 간격을 조정하는 데 사용된다.


### margin 사용법

css
```
.element {
  margin: 20px; /* 모든 방향에 20px 여백 */
}
```

### margin의 다양한 설정 방법

1. 네 방향 동일한 값
```
margin: 10px;
```
+ 모든 방향(상, 우, 하, 좌)에 10px의 여백이 설정됨.

<br>

2. 상하 / 좌우 따로 설정
```
margin: 10px 20px;
```
+ 위아래(10px), 좌우(20px).

<br>

3. 개별적으로 설정 (top right bottom left 순서)
```
margin: 10px 15px 20px 25px;
```
+ 위 10px, 오른쪽 15px, 아래 20px, 왼쪽 25px.

<br>

4. 자동 정렬 (margin: auto;)
```
.container {
  width: 200px;
  margin: auto;
}
```

<br>

5. 개별 속성 사용 (margin-top, margin-right 등)
```
margin-top: 10px;
margin-right: 15px;
margin-bottom: 20px;
margin-left: 25px;
```

<br>

6. 음수 값 사용 가능
```
margin: -10px;
```





