## Switch문 무엇인가
> Switch문 여러 조건을 효율적으로 처리하기 위해 사용하는 조건문이다. 각 case로 구분되며, 참이면, 해당 블록이 실행된다.

### 장점 
+ 조건이 많을 경우, if-else문 보다는 코드가 구조적이라 좋다.
+ 유지보수시 코드가 깔끔하고 읽기도 좋다.

### 단점 
+ 복잡한 조건문이나, 비교 대상이 많으면 if-else가 더 낫다.

<strong>if-else문 사용</strong> 
```
let day = "월요일"

if day == "월요일" {
    console.log("오늘은 월요일 입니다.")
} else if day == "화요일" {
    console.log("오늘은 화요일 입니다.")
} else if day == "수요일" {
    console.log("오늘은 수요일 입니다.")
} else if day == "목요일" {
    console.log("오늘은 목요일 입니다.")
} else if day == "금요일" {
    console.log("오늘은 금요일 입니다.")
} else if day == "토요일" || day == "일요일" {
    console.log("오늘은 주말 입니다.")
} else {
    console.log("좋은 하루 보내세요 ~")
}

```

<strong>switch문 사용</strong>
```
let day = "월요일"

switch day {
case "월요일":
    cpnsole.log("오늘은 월요일 입니다.")
case "화요일":
    console.log("오늘은 화요일 입니다.")
case "수요일":
    console.log("오늘은 수요일 입니다.")
case "목요일":
    console.log("오늘은 목요일 입니다.")
case "금요일":
    console.log("오늘은 금요일 입니다.")
case "토요일", "일요일":
    console.log("오늘은 주말 입니다.")
default:
    console.log("좋은 하루 보내세요 ~ ")
}

```





