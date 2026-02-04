## 📌 react-hook-form
> React에서 폼(Form)을 아주 간단하고 빠르게 관리할 수 있게 도와주는 라이브러리이다.

### 목차
+ 왜 react-hook-form을 쓰나요?
+ react-hook-form 방식
+ 핵심 개념 5가지
+ 전체 예제 (아주 기본)
+ react-hook-form의 장점
+ 언제 쓰면 좋을까?

### ❓ 왜 react-hook-form을 쓰나요?
### ❌ 기존 방식 (useState 지옥)

```
const [email, setEmail] = useState("");
const [password, setPassword] = useState("");
```
+ input마다 state 필요
+ 코드 많아짐
+ 성능도 안 좋음 (리렌더링 많음)

### ✅ react-hook-form 방식
```
const { register } = useForm();
<input {...register("email")} />

```
+ state 직접 관리 ❌
+ 코드 짧음
+ 성능 좋음 🚀

#### 🧠 핵심 개념 5가지
### 1️⃣ useForm()

폼 전체를 관리하는 핵심 Hook
```
const { register, handleSubmit, formState } = useForm();
```

### 2️⃣ register
input을 react-hook-form에 등록
```
<input {...register("email")} />
```
+ 👉 “이 input은 email이야”라고 알려주는 역할

3️⃣ handleSubmit
폼 제출 시 실행되는 함수
```
<form onSubmit={handleSubmit(onSubmit)}>
```
+ ✔️ 유효성 검사 통과 시에만 실행됨


4️⃣ formState.errors
유효성 검사 실패 시 에러 정보
```
{errors.email && <p>이메일은 필수입니다</p>}
```

5️⃣ 유효성 검사 (Validation)
```
<input
  {...register("email", {
    required: "이메일은 필수입니다",
    minLength: { value: 5, message: "5자 이상 입력" },
  })}
/>

```

### 🧪 전체 예제 (아주 기본)
```
import { useForm } from "react-hook-form";

function LoginForm() {
  const { register, handleSubmit, formState: { errors } } = useForm();

  const onSubmit = (data: any) => {
    console.log(data);
  };

  return (
    <form onSubmit={handleSubmit(onSubmit)}>
      <input {...register("email", { required: "이메일 필수" })} />
      {errors.email && <p>{errors.email.message}</p>}

      <button type="submit">로그인</button>
    </form>
  );
}

```

### 🚀 react-hook-form의 장점
+ 성능 좋음	> 불필요한 리렌더링 없음
+ 코드 간결	> useState 거의 안 씀
+ 서버 에러 처리 쉬움	> 백엔드 에러 연동 쉬움
+ Zod / Yup 연동	> 타입 안정성 ↑


### 📌 언제 쓰면 좋을까?

+ 로그인 / 회원가입
+ 글 작성 폼
+ 관리자 페이지
+ 입력 필드 많은 화면




