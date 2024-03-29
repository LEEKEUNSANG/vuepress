# Ajax 개요

## Ajax가 뭐야???

Ajax는 Asynchronous JavaScript and XML(<a href='https://leekeunsang.github.io/vuepress/Study_Ajax/ajax_info/ajax_info.html#%E1%84%87%E1%85%B5%E1%84%83%E1%85%A9%E1%86%BC%E1%84%80%E1%85%B5-%E1%84%90%E1%85%A9%E1%86%BC%E1%84%89%E1%85%B5%E1%86%AB%E1%84%8B%E1%85%B5-%E1%84%86%E1%85%AF%E1%84%8B%E1%85%A3'>비동기식 </a>자바스크립트와 xml)의 약자다. \
JavaScript의 라이브러리 중 하나로
JavaScript를 통해 서버에 데이터를 요청하는 것이다.

- 클라이언트에서 서버로 데이터를 요청하고 그에 대한 결과를 돌려받을 수 있다.

::: tip 요약
백그라운드에서 <a href='https://leekeunsang.github.io/vuepress/Study_Ajax/XMLHttpRequest/XMLHttpRequest.html'>XMLHttpRequest</a> 객체를 이용해 필요한 데이터만 받아 페이지의 일부만을 로드할 수 있다. \
= **새로고침이 필요 없다!!!!**
:::

::: details 서버와 주고받을 수 있는 데이터 형태

- JSON
- XML
- HTML
- TEXT 등
  :::

## Ajax의 장단점

::: tip Ajax의 장점

- 웹 페이지 전체를 리로드하지 않고 웹 페이지의 일부만을 갱신할 수 있다.(빠르다!)
- 서버에서 데이터만 전송한다(가볍다!)
- 웹 페이지가 로드된/로드중인 상태에서 데이터를 주고 받을 수 있다.
- 백그라운드 영역에서 서버로 데이터를 보낼 수 있다.
- UI의 다양성이 증가한다.
  :::

::: danger Ajax의 단점

- 클라이언트가 서버에 데이터를 요청하는 클라이언트 풀링 방식을 사용하므로 서버 푸시 방식의 실시간 서비스는 만들 수 없다.
  ::: warning 클라이언트 풀링? 서버 푸시?
  - 클라이언트 풀링(Client pooling) 방식 : 사용자가 원하는 정보를 서버에 요청하여 얻는 방식(수동적)
  - 서버 푸시(Server push) 방식 : 사용자가 요청하지 않아도 서버가 자동으로 특정 정보를 제공하는 방식(능동적)
    :::
- 바이너리 데이터(이진 파일)를 보내거나 받을 수 없다.
- Ajax 스크립트가 포함된 서버 내에서만 주고 받을 수 있다.(다른 도메인과는 통신이 불가능)
- XMLHttpRequest를 통해 통신하는 경우, 사용자에게 아무런 진행 정보가 주어지지 않는다.
  :::

## Ajax의 진행과정

## 비동기 통신이 뭐야?

- 웹 페이지를 리로드하지 않고 데이터를 불러오는 방식.
- Request를 보낸 Thread는 Response를 기다리지 않고 다른 업무를 처리할 수 있다.
- 필요한 데이터만을 불러와 사용할 수 있어 성능면에서 빠르고 리소스 낭비가 적다.
- <font style='color:red;'>Response의 순서가 Request의 순서와 다를 수 있다.(Response에 대한 처리 결과를 보장받고 처리해야하는 서비스엔 부적합하다.)</font>

<a href='https://leekeunsang.github.io/vuepress/Study_Ajax/ajax_info/ajax_info.html#ajax%E1%84%80%E1%85%A1-%E1%84%86%E1%85%AF%E1%84%8B%E1%85%A3'>돌아가기</a>
