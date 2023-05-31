<details>
  <summary>쿠키란? (4)</summary>
  <br />
  
  - 쿠키(Cookie)는 인터넷 사용자의 컴퓨터나 모바일 장치에 저장되는 작은 데이터 파일입니다. 주로 웹사이트에서 사용되며, 웹사이트를 방문할 때마다 웹 브라우저에 의해 자동으로 생성됩니다. 이 쿠키는 사용자가 웹사이트를 방문할 때마다 다양한 정보를 저장하고 추적합니다.
  - 쿠키는 다양한 용도로 사용됩니다. 예를 들어, 쇼핑몰 웹사이트에서는 쿠키를 사용하여 사용자가 쇼핑 카트에 담은 제품 목록이나 배송지 정보를 저장할 수 있습니다. 또한, 웹사이트의 로그인 정보나 개인화된 설정 등도 쿠키에 저장됩니다.
  - 로그인에 성공했을 때 서버가 `Set-Cookie` 헤더로 쿠키 값을 보내주면 이걸 클라이언트가 저장해 두었다가, 서버에 리퀘스트를 보낼 때마다 매번 `Cookie` 헤더로 보내서 로그인 된 상태라는 걸 표시합니다. 웹 브라우저를 껐다 키거나 컴퓨터를 껐다 키더라도 쿠키 값은 유지되기 때문에 평소에 사이트를 한 번 로그인하면, 일정 기간 동안은 로그인하지 않아도 로그인이 유지됩니다.
  - 쿠키는 일반적으로 개인 식별 정보를 저장하지 않으며, 사용자의 웹 브라우저에서 수동으로 삭제할 수 있습니다. 그러나 쿠키가 개인 정보를 수집하거나 불법적인 방법으로 사용될 수 있는 가능성도 있으므로, 사용자는 웹사이트에서 쿠키 사용에 대한 동의를 결정할 수 있습니다.
</details>

<details>
  <summary>쿠키의 특징 (3)</summary>
  <br />
  
  - 서버로부터 리스폰스로 쿠키를 받으면, 클라이언트에서는 별도로 작업을 해주지 않아도 알아서 웹 브라우저가 알아서 저장하고 리퀘스트를 보낼 때도 웹 브라우저가 알아서 보냅니다.
  - 자바스크립트를 통해서 쿠키 값을 추가, 수정, 참조할 수 있습니다.
  - 수명을 지정할 수 있습니다. 수명이 다한 쿠키는 알아서 지워집니다.
</details>

<details>
  <summary>쿠키 사용법에 대해 설명해주세요. (3)</summary>
  <br />
  
  - 서버에서 리스폰스할 때
    - 서버에서 `set-cookie` 헤더를 리스폰스로 보내주면 웹 브라우저는 알아서 쿠키 값을 저장해 둡니다.
    ```tsx
    Set-Cookie: session-id=1234; Domain=codeit.kr; Path=/; HttpOnly;
    Secure; SameSite=Strice; Max-Age=2592000;
  
    ```
    - 여기서 맨 앞의 `session-id` 는 쿠키의 Key에 해당하는 값이고, `1234` 는 Value에 해당하는 값입니다. `domain`, `path`, `samesite` 등은 쿠키의 Attribute에 해당하는 값입니다.(참고로 위에 적혀있는 헤더 이름이나 Attribute 이름들은 대소문자를 구분하지 않기 때문에 `set-cookie`, `domain`, `path`, `samesite` 로 쓸 수도 있습니다.)
  - 클라이언트에서 보낼 때
    - 리퀘스트를 보낼 때 주소에 해당하는 쿠키가 저장되어 있다면 웹 브라우저가 알아서 쿠키를 보내줍니다.
    ```tsx
    Cookie: session-id:1234; Domain=codeit.kr; Path=/; HttpOnly;
    Secure; SameSite=Strict; Max-Age=2592000;
    
    ```
  - 자바스크립트로 사용하기
    - 보통은 서버가 쿠키 값을 만들고, 클라이언트에서는 웹 브라우저에 맡기고 건드리지 않는 것이 권장됩니다. 하지만 클라이언트에서 자바스크립트로 쿠키를 생성/수정/참조 할 수도 있습니다.
    - 추가, 수정하기
    ```tsx
    document.cookie = "session-id=1234; Domain=codeit.kr; Path=/; HttpOnly; Secure; SameSite=Strict; Max-Age=2592000;";

    ```
      - 변수 할당처럼 보이지만 이 코드는 새로운 쿠키를 추가하거나 (기존에 session-id라는 쿠키가 있다면) 수정하는 코드입니다.
    - 값 참조하기
      - `document.cookie` 값을 참조하면 모든 쿠키의 키와 값이 ; 문자로 구분된 문자열입니다.
      - `split()` 함수를 사용해서 직접 분리해서 사용하거나, 다양한 방법들을 사용할 수 있습니다. [스택오버플로우 링크](https://stackoverflow.com/questions/10730362/get-cookie-by-name)
      - [cookie](https://www.npmjs.com/package/cookie)라는 NPM 패키지를 활용할 수도 있습니다.
    - 값 지우기
      - `Max-Age` 값을 0으로 업데이트하면 수명이 0이 되어 지워집니다.
      ```tsx
      document.cookie = "session-id; Max-Age: 0;";
  
      ```
</details>

<details>
  <summary>쿠키의 Domain attribute란? (1)</summary>
  <br />
  
  - 브라우저가 쿠키를 보낼 도메인을 지정합니다. 예를 들어서 `Domain=codeit.kr` 이라고 하면 `https://codeit.kr` 은 물론이고 `https://abc.codeit.kr`, `https://xyz.abc.codeit.kr` 같은 서브 도메인([서브 도메인이란?](https://kr.godaddy.com/help/what-is-a-subdomain-296))에 리퀘스트를 할 때도 쿠키를 보냅니다.
</details>

<details>
  <summary>쿠키의 HttpOnly attribute란? (2)</summary>
  <br />
  
  - `document.cookie` 값을 자바스크립트로 사용할 수 있으면, 해커들이 악성 코드를 사용자들에게 유포해 쿠키를 훔칠 수 있습니다. ([게시판에 자바스크립트를 올려서 쿠키를 탈취하는 Cross-Site Scription 사례](https://kciter.so/posts/basic-web-hacking#cross-site-scription-xss))
  - 로그인 정보 같은 민감한 정보는 되도록이면 자바스크립트로 조작하면 안됩니다. `HttpOnly` 를 사용하면 쿠키를 자바스크립트로 사용하지 못하게 막을 수 있습니다.
</details>

<details>
  <summary>쿠키의 Secure attribute란? (1)</summary>
  <br />
  
  - `Secure` 를 지정하면 HTTPS 리퀘스트를 보낼 때만 쿠키를 보냅니다. 참고로 `SameSite=None` 을 지정하면 반드시 `Secure`도 함께 지정해야 합니다.
</details>

<details>
  <summary>쿠키의 SameSite attribute란? (2(3))</summary>
  <br />
  
  - [크로스 사이트 요청 위조 (Cross-site request forgery, CSRF, XSRF)](https://ko.wikipedia.org/wiki/%EC%82%AC%EC%9D%B4%ED%8A%B8_%EA%B0%84_%EC%9A%94%EC%B2%AD_%EC%9C%84%EC%A1%B0)를 방지하기 위해서 제3자 사이트(Third-party site)에서 쿠키를 보내지 못하게 `SameSite` 를 지정해야 합니다.
  - `SameSite` 속성의 값에는 `Strict`, `Lax` (아무것도 지정하지 않았을 때 기본값), None이 있습니다.
    - `Strict` 같은 사이트로 리퀘스트르 보낼 때만 쿠키를 전송합니다.
    - `Lax` + 다른 사이트에서 사용자가 링크를 클릭해 우리 사이트로 이동할 때에도 쿠키를 저송합니다.
    - `None` + 다른 사이트에서 우리 사이트로 리퀘스트를 보내거나 이미지 파일 등을 받을 때에도 쿠키를 전송합니다.
</details>

<details>
  <summary>쿠키의 Expires와 Max-Age attribute란? (3)</summary>
  <br />
  
  - 쿠키의 수명을 지정하는 속성입니다. `Expires`로 만료될 시기를 지정하거나, `Max-Age` 로 쿠키의 수명을 지정할 수 있습니다.
  - `세션 쿠키(Session Cookie)` `Expires` 나 `Max-Age` 를 지정하지 않으면 만들 수 있습니다. 세션 쿠키는 브라우저를 닫으면 지워지는 쿠키입니다.
  - `영속적인 쿠키(Persistent Cookie)` `Expries` 나 `Max-Age` 로 수명을 지정해서 만들 수 있습니다. 수명이 다하면 지워지는 쿠키입니다.
</details>

<details>
  <summary>GDRP란? (3)</summary>
  <br />
  
  - 예전에 구글, 페이스북 등 빅테크들이 쿠키를 사용해서 사용자의 정보를 과도하게 수집하고 자사 광고에 활용해 논란이된 적이 있습니다. 그래서 유럽 연합에서는 개인정보의 범위를 넓혀 직간접적으로 개개인을 식별할 수 있는 데이터까지 개인정보로는 규정을 만들게 되었습니다. 여기에는 쿠키 데이터도 포함됩니다.
  - 따라서 쿠키를 사용하는 경우 GDPR(일반 정보 보호 규정; General Data Protection Regulation) 규정에 따르면 개인정보 이용목적을 안내하고 사용자의 동의를 받는 등의 절차가 필요합니다. 그래서 최근 많은 사이트들이 처음 들어가면 팝업을 띄우고 동의를 받습니다.
  - [[모비랩의 테크인사이드] 마케터라면 필수적으로 알아야 할 'GDPR(일반 정보 보호 규정)' 이해 - 모비인사이드 MOBIINSIDE](https://www.mobiinside.co.kr/2018/03/19/mobilab-gdpr/) 참조
</details>

<details>
  <summary>세션 스토리지와 로컬 스토리지의 공통점과 차이점은? (3)</summary>
  <br />
  
  - 세션 스토리지(Session storage)와 로컬 스토리지(Local storage)는 모두 웹 브라우저에서 제공하는 클라이언트 사이드 저장소입니다.
  - 이 두 가지 저장소는 모두 키-값 쌍의 데이터를 저장하고, JavaScript를 사용하여 데이터를 추가, 수정, 삭제 및 검색할 수 있습니다.
  - 세션 스토리지는 데이터를 일시적으로 저장하는 경우에 유용하고, 로컬 스토리지는 영구적으로 데이터를 저장하는 경우에 유용합니다.
</details>

<details>
  <summary>세션 스토리지란? (2)</summary>
  <br />
  
  - 세션 스토리지는 웹 브라우저의 세션 기간 동안 데이터를 저장합니다. 세션 기간 동안에는 사용자가 웹 사이트에 접속하고 브라우저를 종료할 때까지를 의미합니다. 브라우저를 종료하면 세션 스토리지에 저장된 모든 데이터가 삭제됩니다.
  - 현재 탭에서만 유효한 저장소이기 때문에 탭을 닫으면 데이터가 사라지고 다른 탭과 데이터는 공유되지 않습니다.
</details>

<details>
  <summary>로컬 스토리지란? (2)</summary>
  <br />
  
  - 로컬 스토리지는 데이터를 영구적으로 저장합니다. 사용자가 브라우저를 닫아도 데이터는 계속 유지됩니다. 이러한 특징은 사용자가 웹 사이트를 다시 방문할 때 데이터를 유지할 수 있도록 합니다.
  - 해당 사이트에서 유효한 저장소이기 때문에 탭을 닫거나 브라우저를 닫아도 데이터가 유지되고 여러 탭 사이에서도 데이터가 공유됩니다.
</details>

<details>
  <summary>스토리지가 쿠키와 다른 점은? (4)</summary>
  <br />
  
  - 클라이언트가 만들고 관리하는 데이터입니다.
  - 자바스크립트로 편리하게 조작할 수 있습니다.
  - 만료 기간(수명)이 없습니다.
  - 쿠키보다 사용할 수 있는 용량이 큽니다.
</details>

<details>
  <summary>스토리지가 변경되었을 때 javascript 이벤트를 처리하는 방법은? (1)</summary>
  <br />
  
  - 스토리지가 변경되었을 때 `'storage'` 라는 이벤트가 발생합니다.
  ```tsx
  window.addEventListener("storage", () => {
    const showSidebar = localStorage.getItem('show-sidebar') === 'true';
      // showSidebar 값 적용하기
  });

  ```
</details>
