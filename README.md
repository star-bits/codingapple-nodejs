# Node.js, MongoDB로 빠르게 웹서비스 만들기

## P1-2
- js: html 따까리
- 크롬 js 실행 엔진 v8 = nodejs = js 런타임 = js 실행기
- nodejs 장점: non-blocking/비동기처리 잘함 = 시간 오래 걸리는거 만나면 제껴두고 다른거 먼저 함

## P1-3
- `server.js`
- `npm init -y`
- `npm install express`
```js
const express = require('express') // express 라이브러리를
const app = express() // 사용하겠다는 뜻

app.listen(8080, () => { // app.listen(): 포트 오픈하는 문법, 8080: 포트 넘버
    console.log('http://localhost:8080 에서 실행중')
})

app.get('/', (요청, 응답) => { // 메인페이지('/') 접속시
    응답.send('반갑다')
})
```
- 실행: `node server.js`

## P1-4
