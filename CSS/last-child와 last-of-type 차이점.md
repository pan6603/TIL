### last-child
+ 부모 요소의 마지막 자식 요소를 선택한다.
+ 요소의 타입(태그 종류) 은 고려하지 않는다.

### last-of-type
+ 부모 요소 내에서 같은 태그 유형 중 마지막 요소를 선택한다.
+ 다른 태그가 섞여 있어도 같은 유형(<li>)의 마지막 요소만 선택한다.


### last-child 코드

html 
```
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <span>Not an li</span>
  <li>Item 3</li>
</ul>

```

css 
```
li:last-child {
  color: red;
}
```

### last-of-type 코드

html 
```
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <span>Not an li</span>
  <li>Item 3</li>
</ul>

```

css
```
li:last-of-type {
  color: red;
}
```

### 차이점 
+ last-child는 부모의 마지막 자식인지를 확인함 → 요소의 종류(태그 타입) 는 상관없음.
+ last-of-type은 같은 태그 중에서 마지막인지를 확인함 → 다른 태그가 섞여 있어도 마지막 해당 태그만 선택됨.









