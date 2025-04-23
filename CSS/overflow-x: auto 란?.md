## overflow-x: auto 란?
> overflow-x는 가로 방향(수평 방향)의 콘텐츠가 너비를 넘칠 때 스크롤바가 생긴다.

### 사용 이유
긴 내용이 화면 밖으로 나가버리지 않게 스크롤로 처리

### 코드 예제 
```
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <style>
    .box {
      width: 300px;
      height: 100px;
      border: 1px solid #000;
      overflow-x: auto; /* 넘치면 가로 스크롤 생김 */
      white-space: nowrap; /* 줄바꿈 방지 */
    }
  </style>
</head>
<body>

  <div class="box">
    이것은 아주아주아주아주아주아주아주 긴 문장입니다. 이 문장은 넘쳐서 스크롤이 생긴다.
  </div>

</body>
</html>

```


