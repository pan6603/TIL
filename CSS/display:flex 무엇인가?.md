## display:flex 무엇인가?
> CSS에서 Flexbox 레이아웃을 활성화하는 속성입니다. 이를 사용하면 컨테이너(부모 요소) 안에 있는 자식 요소들이 가로 또는 세로로 정렬됩니다.

#### style.css

```
.container {
  display: flex;
}
```

#### index.html 

```
<div class="container">
  <div class="box">1</div>
  <div class="box">2</div>
  <div class="box">3</div>
</div>
```

### Flexbox를 사용할 때의 장점
+ justify-content, align-items를 사용하면 가로, 세로 정렬이 쉬움
+ flex-wrap, flex-grow 등을 활용해 화면 크기에 따라 동적으로 조정 가능. 
