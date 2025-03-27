## box-sizing: border-box란 ? 
> 일반적으로 HTML 요소의 크기는 width와 height 속성으로 정의되지만, 이 크기에 padding과 border가 추가되면서 요소의 실제 크기가 커지는 문제가 발생할 수 있다.
이를 해결하기 위해 box-sizing: border-box;를 사용하면, width와 height에 padding과 border가 포함된 상태로 요소의 크기를 계산한다.

### 언제 사용하면 좋을까?
+ 레이아웃을 깔끔하게 유지하고 싶을 때
+ 여러 요소의 크기를 맞춰야 할 때
+ width와 height를 정확하게 유지하면서 padding과 border를 추가하고 싶을 때

### 전체 요소에 적용하기

css
```
* {
  box-sizing: border-box;
}

```
전체 요소에 모든 요소를 border-box 기준으로 적용하면 크기가 계산되어, 예상치 못한 크기 변경 문제를 방지할 수 있다.

