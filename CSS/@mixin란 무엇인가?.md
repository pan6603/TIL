## @mixin란 무엇인가?
> CSS (정확히는 Sass 또는 SCSS)에서 @mixin은 재사용 가능한 스타일 블록을 정의할 때 사용된다. <br> @mixin 안에서는 일반 CSS 속성뿐 아니라, 변수, 조건문, 반복문 등을 사용할 수 있어 매우 유용하다.

### 사용이유 
 CSS에서 @mixin는 코드의 재사용성, 유지보수의 편리함 때문에 사용한다. 

#### style.scss 
```
@mixin button-style($color) {
  background-color: $color;
  border: none;
  padding: 10px 20px;
  color: white;
  cursor: pointer;
  border-radius: 5px;

  &:hover {
    background-color: darken($color, 10%);
  }
}

.button-primary {
  @include button-style(blue);
}

.button-secondary {
  @include button-style(gray);
}

```

#### index.html 
```

<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <!-- <link rel="stylesheet" href="./style.css"> -->
  <link rel="stylesheet" href="./main.css">
</head>
<body>  
    <button class="button-primary"></button>
    <button class="button-secondary"></button>

    <script src="./main.js"></script>
</body>
</html>
```

### 정리 

+ 재사용성 반복되는 코드를 줄여줌
+ 유지보수성	한 곳에서 수정하면 전부 적용됨
+ 동적 스타일 인자를 활용해 다양한 스타일 구성 가능
+ 가독성 향상 코드가 깔끔하고 구조적으로 정리됨
