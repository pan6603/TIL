## position: relative 이란?
> position: relative;는 HTML 요소를 원래 위치(정적 위치)를 기준으로 이동할 수 있도록 하는 CSS 속성이다.
즉, 기본 위치를 유지하면서 top, left, right, bottom 속성을 사용해 이동할 수 있다.

### 코드 예제

css
```
.container {
    position: relative;
    width: 200px;
    height: 200px;
    background-color: lightgray;
}

.child {
    position: absolute;
    top: 20px;
    left: 20px;
    width: 50px;
    height: 50px;
    background-color: red;
}

```

html

```
<div class="container">
    <div class="child"></div>
</div>

```

+ .child(absolute 요소)는 relative가 적용된 .container를 기준으로 이동.


### 정리 
+ position: relative;는 원래 위치를 기준으로 이동.
+ top, left, right, bottom으로 조정 가능.
+ absolute는	가장 가까운 relative 부모 기준으로 이동하며, 원래 자리에서 빠져나옴.
