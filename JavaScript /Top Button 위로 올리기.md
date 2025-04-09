## Top Button이란?
> topButton은 페이지 위로 올라가기 버튼을 HTML에서 만들기 위해 우리가 직접 붙인 id 이름이다.

#### html 
```
<button id="topButton">↑</button>

```
+ button 만든다.

#### css 
```
#topButton {
  position: fixed;
  bottom: 30px;
  right: 30px;
  width: 50px;
  height: 50px;
  background-color: #87CEFA; /* Light Sky Blue */
  color: white;
  border: none;
  border-radius: 50%;
  font-size: 24px;
  cursor: pointer;
  display: none;
  z-index: 999;
  transition: background-color 0.3s ease;
}

#topButton:hover {
  background-color: #00BFFF; 
}

```

#### js
```
<script>
  const topButton = document.getElementById("topButton");

  window.onscroll = function () {
    if (document.documentElement.scrollTop > 200) {
      topButton.style.display = "block";
    } else {
      topButton.style.display = "none";
    }
  };

  topButton.addEventListener("click", () => {
    window.scrollTo({
      top: 0,
      behavior: "smooth"
    });
  });
</script>

```






