## justify-content 속성이란
> justify-content 속성은 CSS의 Flexbox와 Grid 레이아웃에서 아이템을 가로 또는 세로 방향으로 정렬할 때 사용하는 속성입니다.

### 예제 코드 

1. 기본적인 Flexbox에서 justify-content 사용 

#### style.css
```
.container {
  display: flex;
  justify-content: center; // 중앙 정렬
  background-color: lightgray; 
}
```

#### index.html
```
<div class="container">
   <div class="item">1</div>
   <div class="item">2</div>
   <div class="item">3</div>
</div>
```

2. justify-content: space-between; 사용

#### style.css
```
.container {
  display: flex;
  justify-content: space-between;
}
```
