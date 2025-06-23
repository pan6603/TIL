## fadeInUp 무엇인가?
> fadeInUp는 일반적으로 CSS 애니메이션에서 사용되는 이름으로, 요소가 아래쪽(아래→위)에서 점점 나타나며 올라오는 효과이다.

### 동작 설명
+ 요소의 투명도(opacity)가 0에서 1로 점점 선명해진다(페이드 인).
+ 동시에 요소가 아래에서 위로(translateY로) 이동하며 등장.

css
```
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(40px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.my-fadeInUp {
  animation: fadeInUp 1s ease;
}
```

html 
```
<div class="my-fadeInUp">안녕하세요!</div>
```

### 요약
+ fadeInUp은 요소가 아래에서 위로 올라오며 천천히 나타나는 애니메이션 효과이다.
+ 주로 Animate.css 등에서 클래스 이름으로 사용된다.
+ 직접 CSS로도 구현할 수 있다.
