## React Swiper란?
> Swiper는 이미지 슬라이더나 콘텐츠 캐러셀을 만들 때 사용되며, 터치/마우스 드래그, 자동 슬라이드, 페이지네이션, 네비게이션 등 다양한 기능을 제공한다.

### 🔧 설치
```
npm install swiper

```

### 🔌 사용 예시 (React)
```
import { Swiper, SwiperSlide } from 'swiper/react';
import 'swiper/css';

function MySwiper() {
  return (
    <Swiper
      spaceBetween={30}
      slidesPerView={1}
      loop={true}
      autoplay={{ delay: 3000 }}
      pagination={{ clickable: true }}
    >
      <SwiperSlide>슬라이드 1</SwiperSlide>
      <SwiperSlide>슬라이드 2</SwiperSlide>
      <SwiperSlide>슬라이드 3</SwiperSlide>
    </Swiper>
  );
}

```

### 📦 기능
+ 터치 슬라이드 지원 (모바일 친화적)
+ 자동 슬라이드(autoplay)
+ 무한 반복(loop)
+ 슬라이드 간 간격 조절
+ 네비게이션 버튼 및 페이지네이션
+ 여러 슬라이드 보여주기 (slidesPerView)
+ 반응형 지원


