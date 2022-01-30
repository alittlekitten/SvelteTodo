# 🎃 Svelte + TS + Vite + TailWindCSS

- Svelte-ts와 Vite, TailWindCSS를 이용해서 간단한 TodoList를 만들었습니다.
- 코드의 양이 굉장히 간소화되었고, CSS의 길이도 굉장히 줄었고, 빌드속도 역시 굉장히 빨랐습니다.
- 왜 신문물을 사용하는 지 알 수 있었습니다.

<br />

## 🔧 기술스택

<div>
  <img src="https://img.shields.io/badge/Svelte-FF3E00?style=flat-square&logo=svelte&logoColor=white"/>
  <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white"/>
  <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white"/>
</div>
  
<br />

## 📌 고민한 점

- **Svelte-TS와 TailWindCSS를 연결하는 데에 시간을 많이 사용했습니다.**

  - postcss를 사용해서 해결했습니다.
  - ESM 모듈을 사용했기 때문에 modlue.exports들이 있다면 모두 export default 형식으로 바꿔서 문제를 해결했습니다.

- **웹폰트를 다운받아서 사용했습니다.**

  - import한 후에 `tailwind.config.js`파일의 `font-family` 에 이름을 부여해서 사용할 수 있습니다.
  - body라는 이름에 폰트를 넣었으므로 실제로 사용할 때에는 font-body를 통해서 불러와서 사용할 수 있습니다.

- **양방향 바인딩이 무엇인지 이해했습니다.**
  
  - 데이터 바인딩은 화면에 보이는 데이터와 브라우저 메모리에 있는 데이터를 일치시키는 기법입니다.
  - HTML에서 입력한 내용이 JS에 반영되고, script에서 변경된 내용이 HTML에 적용됩니다.
  - React의 단방향 바인딩만 사용하다가 실제로 양방향 바인딩을 사용하니 이벤트 전달과정이 축소되어 훨씬 사용하기 좋았습니다.

<br />

## 🧨 실행 방법

```
npm i
npm run dev
```

<br />

## 🎞 움짤

![Honeycam 2022-01-28 23-20-20](https://user-images.githubusercontent.com/14370441/151562824-0f670e45-6ecb-45ac-96bf-d0abab55449c.gif)
