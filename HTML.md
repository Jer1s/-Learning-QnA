<details>
<summary>HTML이란? (4)</summary>
<br />

- HTML(HyperText Markup Language)은 웹 페이지와 다양한 온라인 콘텐츠를 제작하는데 활용되는 표준 마크업 언어입니다.
- 웹 개발자는 HTML을 이용하여 콘텐츠의 구조를 설계하며, 웹 브라우저가 어떻게 해당 콘텐츠를 사용자에게 보여줄지를 결정합니다.
- 웹 페이지의 내용, 레이아웃 및 스타일을 지정하는 데 필요한 다양한 HTML 태그(tag)와 속성(attribute)을 활용하여 이러한 작업을 수행합니다.
- HTML은 World Wide Web의 핵심 기술이며, 일반적으로 CSS(Cascading Style Sheets) 및 JavaScript와 같은 다른 웹 기술들과 병행하여 사용됩니다.
</details>

<details>
<summary>하이퍼텍스트란? (4)</summary>
<br />

- 하이퍼텍스트(Hypertext)는 다른 텍스트로의 링크를 포함한 텍스트를 의미하며, 이 링크는 클릭 또는 탭을 통해 접근할 수 있습니다.
- 하이퍼텍스트의 개념은 사용자가 하이퍼링크를 통해 다른 페이지나 문서로 쉽게 이동할 수 있게 하는 World Wide Web의 중요한 구성 요소입니다.
- 하이퍼텍스트는 독자에게 다른 섹션 또는 관련 정보로 이동할 수 있는 비선형적인 문서 작성을 가능하게 하며, 이를 통해 보다 상호작용적이고 동적인 사용자 경험을 제공합니다.
- HTML과 같은 마크업 언어는 개발자가 웹 페이지와 다른 온라인 콘텐츠 간에 하이퍼링크를 생성하는데 주로 사용됩니다.
</details>

<details>
<summary>마크업 언어란? (5)</summary>
<br />

- 마크업 언어(Markup language)는 문서의 구조와 포맷을 정의하는데 컴퓨터에 사용되는 언어입니다.
- 마크업 언어는 문서의 콘텐츠, 예를 들어 텍스트, 이미지, 비디오 등을 어떻게 표시할지 지정하기 위해 특별한 코드를 사용합니다.
- 마크업 언어는 특별한 태그나 괄호, 기호 등을 활용하여 일반 텍스트와 구분하며, 이를 통해 문서의 구조와 포맷을 더욱 명확하게 정의합니다.
- 마크업 언어는 문서의 구조와 포맷을 더욱 명확하게 정의하여, 문서의 가독성을 향상시키고 다른 시스템 간에 문서를 쉽게 공유할 수 있도록 합니다.
- HTML, XML, SGML, Markdown, LaTeX 등의 다양한 마크업 언어가 있으며, 각각 다른 목적으로 사용됩니다.
</details>

<details>
<summary>HTML 버전의 역사 (6.10)</summary>
<br />

- HTML(1991)
  - 최초의 HTML이 웹의 창시자인 Tim Berners-Lee에 의해 개발되었습니다.
- HTML 2.0(1995)
  - HTML의 첫 표준화 버전으로, 웹페이지 작성에 필요한 기본적인 기능들을 포함하고 있습니다.
  - 테이블 생성과 이미지 링크를 통한 콘텐츠 포함 등의 새로운 기능이 도입되었습니다.
- HTML 3.2(1997)
  - 인라인 스타일과 폼 등을 처리할 수 있는 새로운 태그가 추가되었습니다.
- HTML 4.0(1998)
  - 프레임, 스타일 시트, 자바스크립트 등의 새로운 기능을 도입했습니다.
- XHTML 1.0(2000)
  - HTML을 XML의 엄격한 문법에 따라 작성된 버전입니다.
- HTML5(2014)
  - 페이지를 더욱 동적이고 인터랙티브하게 만들 수 있는 다양한 새로운 기능과 태그를 도입하였습니다.
  - 비디오, 오디오, 캔버스, 지리 정보 등의 다양한 콘텐츠를 쉽게 표현할 수 있도록 지원합니다.
  - HTML5는 현재 가장 널리 사용되는 HTML 버전이며, 대다수의 웹 브라우저 제조사와 W3C(World Wide Web Consortium)에서 지원합니다.
  - 이를 통해 개발자들은 HTML5를 활용하여 사용자에게 보다 풍부하고 혁신적인 웹 경험을 제공할 수 있습니다.
</details>

<details>
<summary>일부 웹 브라우저에서 HTML 문서의 한글 텍스트가 깨지는 이유 (2)</summary>
<br />

- 웹 브라우저가 인코딩을 정확히 인식하지 못하거나, 텍스트의 인코딩과 브라우저의 인코딩이 일치하지 않을 때 한글 문자가 제대로 표시되지 않을 수 있습니다.
- HTML 문서는 대체로 UTF-8 또는 다른 문자 인코딩 방식을 사용하여 저장됩니다. 이 인코딩은 HTML 문서에 포함된 문자를 컴퓨터가 이해할 수 있는 바이너리 코드로 변환하는 역할을 합니다.
</details>

<details>
<summary>위의 문제를 해결하시오 (1)</summary>
<br />

- HTML 문서의 `<head>` 섹션에 `charset` 속성을 추가하여 문서의 문자 인코딩을 명시적으로 설정할 수 있습니다.
  ```html
  <head>
    <meta charset="UTF-8">
    <title>문서 제목</title>
  </head>
  ```
</details>

<details>
<summary>웹 브라우저 인코딩이란? (5)</summary>
<br />

- 웹 브라우저 인코딩(Web Browser Encoding)은 웹 브라우저가 웹상에서 전송되는 텍스트 데이터를 어떻게 해석하고 표현할지를 결정하는 규칙을 말합니다.
- 인코딩은 특정 문자 집합(Character Set)을 바이트 단위로 변환하는 과정입니다. 이 문자 집합은 컴퓨터에서 인식 및 표현 가능한 문자들의 집합으로, 각 문자는 고유한 코드 값으로 매핑되어 있습니다. 한 예로, 한글은 유니코드(Unicode)에서 U+AC00부터 U+D7AF까지의 코드 범위에 해당하는 코드 값을 가지고 있습니다.
- 웹 페이지는 대체로 HTML, CSS, JavaScript 등의 텍스트 데이터로 이루어져 있습니다. 이러한 텍스트 데이터는 특정 문자 집합을 기반으로 작성되고, 웹 브라우저는 이를 해석하여 사용자에게 웹 페이지를 표시합니다.
- 웹 브라우저 인코딩은 웹 페이지의 텍스트 데이터를 바이트로 변환하는 데 사용되는 인코딩 방식을 결정합니다. 대부분의 웹 브라우저는 UTF-8 인코딩을 기본값으로 사용합니다. UTF-8은 전 세계 모든 언어의 문자를 표현할 수 있는 유니코드 인코딩 방식 중 하나이며, 인터넷에서 널리 사용됩니다.
- 그러나 일부 웹 페이지는 다른 인코딩 방식을 사용할 수도 있습니다. 이 경우, 사용자는 웹 브라우저의 인코딩 설정을 변경하여 해당 인코딩 방식으로 웹 페이지를 제대로 해석할 수 있습니다.
</details>

<details>
<summary>UTF-8이란? (4)</summary>
<br />

- UTF-8은 텍스트를 컴퓨터 시스템에서 표현하고 저장하는 데 널리 사용되는 문자 인코딩 표준입니다.
- 이 인코딩 방식은 가변 길이를 사용하며, 각 문자를 해당하는 유니코드 코드 포인트에 따라 1바이트에서 4바이트까지의 공간에 표현할 수 있습니다.
- UTF-8은 ASCII와의 하위 호환성을 갖추도록 설계되었습니다. 이는 첫 128개의 코드 포인트(ASCII 문자에 해당하는 부분)를 한 바이트로 표현할 수 있음을 의미합니다. 이러한 설계 덕분에, ASCII 문자를 주로 사용하는 언어의 텍스트 처리는 매우 효율적이며, 동시에 다른 문자 체계와 언어의 문자를 유연하게 표현할 수 있습니다.
- UTF-8은 현재 웹 상에서 가장 널리 사용되는 인코딩 방식으로 자리 잡아 있습니다. 거의 모든 최신 웹 브라우저와 운영 체제가 이를 지원하며, 다양한 프로그래밍 언어와 데이터베이스 시스템에서도 활용되고 있습니다. 이로 인해 UTF-8은 웹 및 애플리케이션 개발에서 국제적으로 인식받는 표준으로서의 위치를 확립하였습니다.
</details>

<details>
<summary>HTML 파일의 기본 구조란? (1)</summary>
<br />

```html
<!DOCTYPE html>
<html>
  <head>
  </head>
  <body>
  </body>
</html>
```
</details>

<details>
<summary>&lt&#33DOCTYPE html&gt이란? (6.1)</summary>
<br />

- <\!DOCTYPE html>은 HTML5 문서 유형 선언(doctype declaration)입니다.
- 이 선언은 HTML5에서 문서가 사용하는 버전을 명시하는 역할을 합니다.
- 명시적으로 선언하지 않으면 브라우저가 페이지를 렌더링할 때 자동으로 quirks mode로 동작할 수 있으므로 <\!DOCTYPE html>을 사용하여 명시적으로 문서 유형을 선언하는 것이 좋습니다.
  - 이전 버전의 HTML에서는 `quirks mode`와 `strict mode`라는 두 가지 모드가 있었습니다. `quirks mode`는 이전 버전의 HTML에서 사용되는 레이아웃 동작 방식을 따르는 모드였고, `strict mode`는 최신 표준을 따르는 모드였습니다. 
- <\!DOCTYPE html>은 HTML5 문서에서 항상 사용되는 유일한 선언입니다.
- <\!DOCTYPE html>을 문서의 가장 위에 위치시키는 것이 좋습니다.
- 이전 버전의 HTML에서는 문서 유형 선언이 더 긴 형식으로 작성되었습니다.
</details>

<details>
<summary>태그(Tag)란? (2)</summary>
<br />

- HTML에서 태그는 웹 페이지의 다양한 요소를 정의하는 데 사용되는 중요한 구성 요소입니다. 이 태그들은 꺾쇠 괄호(angle bracket)로 감싸진 키워드를 사용하여 표현됩니다.
- 대부분의 태그는 시작 태그와 종료 태그로 구성되어 있으며, 이 두 태그 사이에 위치한 내용을 감싸서 해당 내용에 대한 정보를 제공합니다. 시작 태그는 `<tag>` 형태로 작성되며, 종료 태그는 `</tag>` 형태로 작성됩니다.
</details>

<details>
<summary>단일 태그(single tag)란? (3)</summary>
<br />

- 빈 요소(empty element)라고도 부릅니다.
- 종료 태그가 필요하지 않습니다.
- 태그 마지막에 슬래시(`/`) 기호를 넣어서 단일 태그라는 표시를 할 수도 있습니다. (이전 버전의 HTML 문법입니다.)
</details>

<details>
<summary>단일 태그의 예시를 드시오. (6)</summary>
<br />

- `<br>` 줄 바꿈을 생성하는 태그
- `<img>` 이미지를 삽입하는 태그
- `<input>` 사용자 입력 필드를 생성하는 태그
- `<meta>` 웹 페이지의 메타데이터를 정의하는 태그
- `<link>` 현재 문서와 외부 리소스를 연결하는 태그
- `<hr>` 수평선을 그리는 태그
</details>

<details>
<summary>태그 속성(attribute)이란? (6)</summary>
<br />

- HTML 태그에 추가 정보를 제공하는 데 사용됩니다.
- 속성은 일반적으로 `(attribute name) = (attribute value)`의 형식으로 작성됩니다.
- HTML에서 속성 이름은 대소문자를 구분하지 않으나, 일관성과 가독성을 위해 대부분 소문자로 작성됩니다.
- 예시
- 일부 속성은 Boolean 속성으로, 해당 속성의 존재 여부만으로 참/거짓을 판단합니다.
- Boolean 속성 예시
  - `checked` 체크박스나 라디오 버튼이 선택되어 있는지 여부를 나타냅니다.
  - `disabled` 입력 필드나 버튼 등이 비활성화되어 있는지 여부를 나타냅니다.
  - `readonly` 입력 필드가 읽기 전용인지 여부를 나타냅니다.
  - `required` 입력 필드가 필수 입력 필드인지 여부를 나타냅니다.
  - `hidden` 요소가 숨겨져 있는지 여부를 나타냅니다.
  - `muted` 미디어 요소가 자동으로 음소거되도록 지정합니다.
</details>

<details>
<summary>태그 속성의 예시를 드시오. (6)</summary>
<br />

- `class` 요소에 대한 CSS 클래스 이름을 지정합니다.
- `id` 요소의 고유한 식별자를 지정합니다.
- `style` 요소에 대한 인라인 CSS 스타일을 지정합니다.
- `title` 요소에 대한 추가 정보(툴팁)를 제공합니다.
</details>

<details>
<summary>Boolean attribute의 예시를 드시오. (6)</summary>
<br />

- `checked` 체크박스나 라디오 버튼이 사용자에 의해 선택되었는지 나타냅니다.
- `disabled` 입력 필드나 버튼 등의 요소가 비활성화되어 있음을 나타냅니다.
- `readonly` 입력 필드가 사용자에 의해 수정될 수 없는 읽기 전용 상태임을 나타냅니다.
- `required` 입력 필드가 사용자로부터 반드시 값을 입력받아야 하는 필수 입력 필드임을 나타냅니다.
- `hidden` 요소가 웹 페이지에서 숨겨져 있음을 나타냅니다.
- `muted` 미디어 요소(`<video>`, `<audio>`)가 자동으로 음소거되도록 지정합니다.
</details>

<details>
<summary>사용자 정의 속성이란? (5)</summary>
<br />

- 사용자 정의 속성(Custom attributes)는 개발자가 HTML 요소에 원하는 속성을 추가하도록 허용하는 방법입니다.
- 이러한 속성은 `data-*` 형식으로 정의되며, 여기서 `*` 부분은 사용자가 임의로 정한 이름이 들어갑니다. 이렇게 정의한 사용자 정의 속성은 JavaScript를 이용해 요소를 조작하거나, CSS를 이용해 스타일을 적용하는 데 사용할 수 있습니다.
- `data-` 접두사를 사용하면, 개발자가 자유롭게 이름을 지정할 수 있는 반면, 표준 속성과 충돌하지 않습니다. 이 접두사를 사용하지 않고 속성을 정의하면, 나중에 표준 HTML 속성에 같은 이름이 추가되었을 때 예기치 못한 결과를 초래할 수 있습니다.
- 사용자 정의 속성은 W3C에서 규정한 HTML 규약에 따라 작성되어야 합니다. 그렇지 않으면, 문서가 유효하지 않다고 판단될 수 있습니다.
- 사용자 정의 속성은 대부분의 현대 브라우저에서 지원되지만, 오래된 브라우저나 일부 특정 브라우저에서는 지원되지 않을 수 있습니다. 따라서 사용자 정의 속성을 사용할 때는 브라우저 호환성에 주의해야 합니다.
</details>

<details>
<summary>HTML tags는 어떤 것들이 있나요?</summary>
<br />

- [HTML elements reference - HTML: HyperText Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element) 참조
</details>

<details>
<summary>&ltmeta http-equiv="X-UA-Compatible" content="IE=edge, chrome=1"&gt가 의미하는 바는 무엇인가요? (3.2)</summary>
<br />

- 이 메타 태그는 웹 페이지를 렌더링하는 데 사용되는 인터넷 익스플로러(IE)의 버전을 지정합니다.
- `http-equiv` 속성은 HTTP 헤더 필드의 이름을 지정합니다.
- `content` 속성은 해당 HTTP 헤더 필드의 값을 지정합니다.
  - `edge` 값은 브라우저가 사용자의 컴퓨터에 설치된 최신 IE 버전을 사용하도록 지시합니다.
  - `chrome=1` 값은 Google Chrome Frame이 설치된 경우 해당 플러그인을 사용하여 웹 페이지를 렌더링하도록 지시합니다.

</details>

<details>
<summary>&ltmeta name="viewport" content="width=device-width, initial-scale=1.0"&gt가 의미하는 바는 무엇인가요? (3.2)</summary>
<br />

- 이 메타 태그는 웹 페이지의 뷰포트를 설정하여 웹 페이지가 다양한 기기에서 어떻게 표시되는지 제어합니다. 이는 특히 모바일 기기에서 웹 페이지가 적절하게 표시되도록 하는 데 중요합니다.
- `name` 속성은 메타데이터의 유형을 지정합니다.
- `content` 속성은 해당 메타데이터의 값을 지정합니다.
  - `width=device-width` 값은 뷰포트의 너비를 현재 기기의 화면 너비로 설정합니다.
  - `initial-scale=1.0` 값은 초기 화면의 줌 레벨을 1.0으로 설정합니다, 이는 웹 페이지가 처음 로드될 때 100%의 화면 크기로 표시되도록 합니다.
</details>

<details>
<summary>&ltmeta name="robots" content="noindex"&gt가 의미하는 바는 무엇인가요? (3)</summary>
<br />

- 이 메타 태그는 검색 엔진 크롤러에게 해당 문서를 인덱싱하지 않도록 지시하는 역할을 합니다.
- `content` 속성의 값으로 `noindex`를 설정하면, 검색 엔진은 해당 페이지를 검색 결과에 포함시키지 않습니다.
- 이 메타태그는 일시적인 페이지, 개발 중인 페이지, 미완성 페이지 등에서 사용할 수 있습니다.
</details>

<details>
<summary>메타 태그(Meta tag)란? (5.2)</summary>
<br />

- 메타 태그(meta tag)는 HTML 문서의 `<head>` 섹션에 위치하는 태그로, 웹 페이지의 메타데이터(meta data)를 정의하는 데 사용됩니다. 이들은 웹 페이지가 어떻게 설명되고, 인덱싱되며, 그 외에도 다양한 속성이 어떻게 적용되는지를 지정합니다.
- 메타데이터는 문서에 대한 부가 정보로, 웹 페이지의 제목(title), 설명(description), 작성자(author), 키워드(keywords), 문자 인코딩(charset) 등을 포함합니다. 이 정보들은 웹 브라우저, 검색 엔진 등에 의해 활용됩니다.
- 메타 태그는 검색 엔진 최적화(SEO)에 중요한 역할을 수행합니다. 검색 엔진은 메타 태그에 포함된 정보를 분석하여 웹 페이지의 내용을 이해하고, 그에 따라 검색 결과를 생성합니다.
- 예시
  - `<meta name="description" content="웹 페이지 설명">` 이 메타 태그는 웹 페이지의 요약 설명을 제공합니다. 이 설명은 검색 엔진 결과 페이지(SERP)에서 보통 페이지 미리보기로 표시됩니다.
  - `<meta http-equiv="refresh" content="5;url=https://example.com">` 이 메타 태그는 웹 페이지가 로드된 후 5초 후에 사용자를 `https://example.com`로 리다이렉트합니다.
- 메타 태그는 웹 브라우저가 웹 페이지를 적절히 해석하고 표시하는 데 도움이 되며, 웹 개발자가 특정 동작을 제어하거나 문서에 대한 정보를 제공하는 데 사용합니다.
</details>

<details>
<summary>오픈그래프(Open Graph)란? (4.3)</summary>
<br />

- 웹 사이트가 소셜 미디어에서 공유될 때 정보를 제공하는 메타데이터 프로토콜입니다.
- 웹 사이트의 메타데이터를 Open Graph 프로토콜로 구성하면, 해당 웹 사이트의 콘텐츠가 소셜 미디어에서 공유될 때 해당 페이지의 제목, 설명, 이미지 등이 더욱 깔끔하게 보여질 수 있습니다.
- 예시
  ```html
  <html>
    <head>
      <meta property="og:title" content="페이지 제목">
      <meat property="og:url" content="페이지 주소">
      <meta property="og:image" content="이미지 URL">
      <meta propery="og:type" content="페이지 타입(ex. website)">
      <meta property="og:description" content="페이지 설명">
    </head>
  </html>
  ```
- Facebook Object Debugger로 디버깅할 수 있습니다.
  - [Facebook Object Debugger](https://developers.facebook.com/tools/debug/)
  - [Open Graph protocol](https://ogp.me/)
</details>

<details>
<summary>Twitter cards란? (4)</summary>
<br />

- 웹 사이트가 Twitter에서 공유될 때 노출되는 정보를 제공하는 메타데이터 프로토콜입니다.
- 웹 사이트의 메타데이터를 Twitter Cards 프로토콜로 구성하면, 해당 웹 사이트의 콘텐츠가 twitter에서 공유될 때 해당 페이지의 제목, 설명, 이미지 등이 더욱 깔끔하게 보여질 수 있습니다.
- 예시
  ```html
  <html>
    <head>
      <meta name="twitter:card" content="summary_large_image">
      <meta name="twitter:site" content="@사이트명">
      <meta name="twitter:title" content="제목">
      <meta name="twitter:description" content="설명">
      <meta name="twitter:image" content="이미지 URL">
    </head>
  </html>
  ```
- Twitter cards validator로 디버깅할 수 있습니다.
  - **[Twitter cards validator](https://cards-dev.twitter.com/validator/)**
</details>

<details>
<summary>구글 애널리틱스란? (3)</summary>
<br />

- 구글 애널리틱스(Google Analytics)는 Google이 제공하는 웹 분석 서비스로, 웹사이트 및 애플리케이션의 트래픽을 추적하고 분석하는 데 사용됩니다.
- 이 도구를 사용하면, 웹사이트나 애플리케이션의 사용자 행동, 방문자 분포, 트래픽 흐름 등 다양한 통계적 데이터를 수집하고 분석할 수 있습니다. 이렇게 수집된 데이터는 웹사이트나 애플리케이션의 성능을 평가하고, 사용자 경험을 개선하며, 마케팅 전략을 구성하는 데에 필수적인 정보를 제공합니다.
- Google Analytics를 사용하려면, Google Analytics 트래킹 코드를 웹사이트나 애플리케이션에 삽입해야 합니다. 이 코드는 방문자의 행동을 추적하고 해당 정보를 Google Analytics에 전송하는 역할을 합니다.
</details>

<details>
<summary>하이퍼링크(Hyperlink)란? (4)</summary>
<br />

- 하이퍼링크(Hyperlink)는 웹 페이지에서 클릭 가능한 링크를 의미합니다.
- 사용자가 이 링크를 클릭하면 해당 웹 페이지나 문서, 이미지, 비디오, 음악 파일 등 다른 컨텐츠로 이동할 수 있습니다.
- HTML에서 클릭 가능한 텍스트를 만들기 위해서는 `<a>` 태그를 사용합니다.
</details>

<details>
<summary>&lta&gt 태그의 타겟 속성이란? (6.1)</summary>
<br />

- `<a>` 태그의 타겟(target) 속성은 링크된 페이지를 어떻게 열지 지정하는 데 사용됩니다.
- `_self` 링크된 페이지를 현재 창 또는 탭에서 엽니다(기본값).
- `_blank` 링크된 페이지를 새 창이나 탭에서 엽니다.
- `_parent` 현재 프레임의 상위 프레임에서 링크된 페이지를 엽니다.
- `_top` 현재 모든 프레임을 새로운 창 또는 탭으로 대체하고, 링크된 페이지를 엽니다.
- `framename` 링크된 페이지가 지정된 이름을 가진 프레임 또는 iframe에 로드됩니다.
  - 하지만 frame은 검색 엔진 최적화(SEO)에 좋지 않은 영향을 미칠 수 있고, 일부 브라우저에서는 더 이상 지원되지 않을 수 있습니다. 그러므로 최신 웹 개발에서는 `<iframe>`보다는 다른 방식을 사용하는 것이 좋습니다.
</details>

<details>
<summary>URL이란? (2)</summary>
<br />

- URL(Uniform Resource Locator)은 URI의 한 형태로, 인터넷에서 리소스의 위치를 나타냅니다.
- URL은 scheme, 프로토콜, 호스트명, 포트 번호, 경로, 쿼리를 포함할 수 있습니다.
</details>

<details>
<summary>URI란? (1)</summary>
<br />

- URI(Uniform Resource Identifier)는 인터넷에서 특정한 리소스를 나타내는 유일한 식별자입니다.
</details>

<details>
<summary>URI의 구조는 어떻게 되나요? (1.7.18)</summary>
<br />

- `scheme:[//[user:password@]host[:port]][/]path[?query][#fragment]`
  - `URI Scheme`
    - URI를 구분하는 스키마(프로토콜)를 나타냅니다.
    - 예를 들어, `http`, `https`, `ftp`, `mailto`, `tel` 등이 있습니다.
    - 각 스키마는 특정 프로토콜을 사용하여 리소스에 접근하는 방법을 정의합니다.
    - 예를 들어, "http://"는 웹 서버에 접근하는 프로토콜을 나타냅니다.
    - IANA의 [URI Scheme list](https://www.iana.org/assignments/uri-schemes/uri-schemes.xhtml) 참조
  - `user:password@`
    - 선택적으로 사용되며, 인증 정보를 나타냅니다.
  - `host`
    - 리소스를 호스팅하는 호스트 이름을 나타냅니다.
    - 예를 들어, "www.example.com"과 같은 도메인 이름을 사용할 수 있습니다.
  - `port`
    - 선택적으로 사용되며, 리소스에 접근하는 데 사용되는 포트 번호를 나타냅니다.
    - 각 프로토콜은 기본 포트를 가지고 있으며, 명시적으로 다른 포트를 사용할 때에만 지정됩니다. 예를 들어, "80"은 HTTP의 기본 포트이고, "443"은 HTTPS의 기본 포트입니다.
  - `path`
    - 리소스의 경로를 나타냅니다.
    - 서버 내부의 파일 경로 또는 RESTful API 엔드포인트 등이 될 수 있습니다.
    - 예를 들어, "/index.html"과 같은 경로를 사용할 수 있습니다.
  - `query`
    - 선택적으로 사용되며, 리소스에 대한 추가적인 정보를 전달하는 데 사용됩니다.
    - 주로 웹 서버에 파라미터를 전달하는데 사용되며, "key=value"와 같은 형식으로 작성됩니다.
  - `fragment`
    - 선택적으로 사용되며, 리소스의 특정 부분을 나타내는 앵커를 나타냅니다.
    - 웹 페이지에서 특정 섹션 또는 위치로 바로 이동할 때 사용됩니다.
    - 예를 들어, "#section1"과 같이 사용합니다.
</details>

<details>
<summary>Text tag는 어떤 것이 있나요? (11)</summary>
<br />

- `<h1>~<h6>` 제목 태그
- `<p>` 본문
- `<br>` 줄바꿈
- `<strong>` 중요(bold)
- `<em>` 강조(italics)
- `<s>` 취소 선
- `<blockquote>/<q>` 긴/짧은 인용(quote)
- `<sub>/<sup>` 아래/위 첨자
- `<hr>` 주제 전환(Horizontal Line)
- `<pre>` Preformatted Text
- `<code>` 짧은 코드
</details>

<details>
<summary>List tag에 대해 설명해주세요. (6)</summary>
<br />

- `<ol>` 순서 있는 리스트(Ordered List)를 나타냅니다.
- `<ul>` 순서 없는 리스트(Unordered List)를 나타냅니다.
- `<li>` 리스트 항목(List Item)을 나타냅니다.
- `<ol>` type attribute
   - `1`, `a`, `A`, `i`, `I` 등
- `<ul>` type attribute
   - `disc`, `circle`, `square` 등
- `<ol>`, `<ul>`에 `list-style` property를 활용할 수 있습니다.
  - `list-style: list-style-type list-style-position list-style-image`
</details>

<details>
<summary>table tag에 대해 설멍해주세요. (9)</summary>
<br />

- `<table>` 표를 만드는 데 사용되는 태그입니다.
- `<caption>` 표의 캡션을 정의합니다.
- `<thead>` 표의 헤더 역할을 하는 부분을 정의합니다.
- `<tbody>` 표의 주요 내용을 나타내는 부분을 정의합니다.
- `<tfoot>` 표의 요약 부분을 정의합니다. 
- `<tr>` 각 표의 행(row)을 나타냅니다.
- `<td>` 각 행의 셀(cell)을 나타냅니다.
- `<th>` 각 열의 제목 셀을 나타냅니다. 브라우저에 따라 bold, center align으로 처리됩니다.
- 예시
  ```html
  <table>
    <caption>이번 달 지출 내역</caption>
    <thead>
      <tr>
        <th>날짜</th>
        <th>지출 내용</th>
        <th>금액</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>4/1</td>
        <td>점심</td>
        <td>10,000원</td>
      </tr>
      <tr>
        <td>4/3</td>
        <td>지하철 요금</td>
        <td>1,250원</td>
      </tr>
      <tr>
        <td>4/6</td>
        <td>생필품 구입</td>
        <td>30,000원</td>
      </tr>
    </tbody>
    <tfoot>
      <tr>
        <td colspan="2">총 지출</td>
        <td>41,250원</td>
      </tr>
    </tfoot>
  </table>
  ```
</details>

<details>
<summary>&lttable&gt에 사용할 수 있는 border 관련 속성(property) 두 가지는 무엇인가요? (2.4)</summary>
<br />

- `border-collapse` 속성은 인접한 셀의 경계선을 병합할 것인지 여부를 결정합니다.
  - `collapse`(기본값) 속성은 인접한 셀의 경계선을 병합합니다. 이 때, 인접한 셀들의 경계선이 중복되지 않습니다.
  - `separate` 속성은 인접한 셀의 경계선을 병합하지 않습니다. 이 때, 인접한 셀들의 경계선이 중복됩니다.
- `border-spacing` 속성은 인접한 셀 간의 간격을 설정합니다.
  - `border-collapse` 속성의 값이 separate인 경우에만 적용됩니다.
  - 이 속성의 값은 길이 또는 백분율로 지정할 수 있습니다. 양수 값으로 지정하여 인접한 셀 간의 간격을 늘리고, 음수 값으로 지정하여 간격을 줄일 수도 있습니다.
</details>

<details>
<summary>img 태그란? (6)</summary>
<br />

- 이미지를 삽입하는 태그입니다.
- 닫는 태그가 없으며, 이미지의 소스를 지정하는 src 속성이 필수적으로 필요합니다.
- `src` 이미지 파일의 경로를 지정합니다. 경로는 상대 경로나 절대 경로 모두 사용할 수 있습니다.
- `alt` 이미지가 로드되지 못했을 때 대신 표시할 텍스트를 지정합니다. 스크린 리더와 같은 보조 기술을 사용하는 사용자들에게 이미지에 대한 정보를 제공하기 위해 사용됩니다.
- `<img>` 태그는 기본적으로 가로폭과 세로폭이 이미지의 크기에 따라 자동으로 설정됩니다. 그러나 width와 height 속성을 사용하여 이미지의 크기를 수동으로 조정할 수도 있습니다.
- 예시
  ```html
  <img src="이미지 경로" alt="대체 텍스트" width="100" height="100">
  ```
</details>

<details>
<summary>video 태그란? (9)</summary>
<br />

- HTML5에서 도입된 태그로, 동영상 콘텐츠를 삽입하는 데 사용됩니다.
- 닫는 태그가 필요하며, 비디오의 소스를 지정하는 src 속성이 필수적으로 필요합니다.
- `src` 비디오 파일의 경로를 지정합니다. 여러 개의 비디오 포맷을 지원하는 브라우저를 대비해, 두 개 이상의 소스를 지정할 수도 있습니다.
- `width`, `height` 비디오의 가로폭과 세로폭을 지정합니다.
- `controls` 비디오 플레이어에 컨트롤러를 표시합니다. 이 속성을 생략하면 컨트롤러가 표시되지 않습니다.
- `autoplay` 비디오가 로드되자마자 자동으로 재생됩니다. 브라우저에 따라 muted 속성이 있어야 autoplay 속성을 사용할 수 있습니다. (Chrome)
- `muted` 비디오가 음소거 상태로 재생됩니다. 
- `<video>` 태그는 다른 요소와 함께 사용하여 비디오를 더욱 풍부하게 표현할 수 있습니다. 예를 들어, `<source>` 요소를 사용하여 동영상 파일의 다양한 포맷을 지정할 수 있습니다. 또한, `<track>` 요소를 사용하여 자막이나 캡션을 추가할 수도 있습니다.
- 예시
  ```html
  <video width="640" height="360" controls muted autoplay>
    <source src="비디오 파일 경로.mp4" type="video/mp4">
    <source src="비디오 파일 경로.webm" type="video/webm">
    <track label="한국어 자막" kind="subtitles" srclang="ko" src="자막 파일 경로.vtt">
    <track label="영어 자막" kind="subtitles" srclang="en" src="자막 파일 경로.vtt">
  </video>
  ```
</details>

<details>
<summary>audio 태그란? (8)</summary>
<br />

- HTML5에서 도입된 태그 중 하나로, 웹 페이지에서 오디오 콘텐츠를 재생하는 데 사용됩니다.
- `src` 오디오 파일의 경로를 지정합니다. 여러 개의 비디오 포맷을 지원하는 브라우저를 대비해, 두 개 이상의 소스를 지정할 수도 있습니다.
- `controls` 오디오 플레이어에 컨트롤러를 표시합니다. 이 속성을 생략하면 컨트롤러가 표시되지 않습니다.
- `autoplay` 오디오가 로드되자마자 자동으로 재생됩니다. 브라우저에 따라 muted 속성이 있어야 autoplay 속성을 사용할 수 있습니다. (Chrome)
- `muted` 오디오가 음소거 상태로 재생됩니다.
- `loop` 반복 재생을 설정합니다.
- `width`, `height` 속성이 없습니다.
- 예시
  ```html
  <audio controls muted autoplay loop>
    <source src="audio.mp3" type="audio/mpeg">
    <source src="audio.ogg" type="audio/ogg">
    <source src="audio.wav" type="audio/wav">
    Your browser does not support the audio element.
  </audio>
  ```
</details>

<details>
<summary>iframe 태그란? (7)</summary>
<br />

- 웹 페이지 내에서 다른 웹 페이지나 독립적인 HTML 문서를 삽입하는 데 사용됩니다.
- 닫는 태그가 필요하며, 삽입할 문서의 URL을 지정하는 src 속성이 필수적으로 필요합니다.
- `src` 삽입할 문서의 URL을 지정합니다.
- `width`, `height` 삽입된 문서의 크기를 조절합니다.
- `frameborder` 테두리를 표시합니다.
- `allowfullscreen` iframe 내에서 전체 화면 재생을 허용할 수 있습니다.
- 예시
  ```html
  <iframe src="https://www.example.com" width="500" height="500"></iframe>
  ```
</details>

<details>
<summary>form 태그란? (3)</summary>
<br />

- 웹 페이지에서 사용자로부터 데이터를 수집하기 위한 양식을 정의하는 데 사용됩니다.
- `<form>` 태그는 다른 HTML 요소들을 포함할 수 있으며, 이러한 요소들은 사용자가 입력할 수 있는 입력 필드, 제출 버튼, 선택 상자, 라디오 버튼 등입니다.
- 사용자가 `<form>` 태그에 데이터를 입력하면, 이러한 데이터는 보통 웹 서버로 전송되어 처리됩니다.
</details>

<details>
<summary>form 태그의 attribute는 어떤 것이 있나요? (5)</summary>
<br />

- `action` 폼 데이터를 전송할 URL을 지정합니다.
- `method` HTTP 요청 방법을 지정합니다. 일반적으로 GET 또는 POST 값을 갖습니다.
- `target` 폼 데이터를 전송한 후 결과를 표시할 위치를 지정합니다.
- `enctype` 폼 데이터를 서버로 전송할 때 사용되는 인코딩 유형을 지정합니다. 기본값은 application/x-www-form-urlencoded 입니다.
- `autocomplete` 자동 완성을 사용할지 여부를 지정합니다. on 또는 off 값을 갖습니다.
</details>

<details>
<summary>input 태그란? (2)</summary>
<br />

- 사용자가 데이터를 입력할 수 있는 입력 필드를 만드는 데 사용됩니다.
- `<input>` 태그는 다양한 종류의 입력 필드를 만들 수 있습니다. 예를 들어, 텍스트 입력 필드, 비밀번호 입력 필드, 라디오 버튼, 체크박스, 파일 업로드 필드 등이 있습니다.
</details>

<details>
<summary>input 태그와 label 태그를 연결하는 방법은? (2)</summary>
<br />

- input 태그의 id를 label 태그의 for 속성값으로 주면 됩니다.
- input 태그를 label 태그 내부에 넣으면 됩니다.
</details>

<details>
<summary>input 태그의 attribute는 어떤 것이 있나요? (7)</summary>
<br />

- `type` 입력받을 데이터의 유형을 지정합니다. 
- `name` 입력받은 데이터의 이름을 지정합니다. 서버로 전송될 때 데이터를 식별하는 데 사용됩니다.
- `value` 입력받은 데이터의 값입니다. `type` 속성값에 따라 다르게 사용됩니다.
- `placeholder` 입력 필드 내부에 힌트 또는 예시를 제공합니다.
- `required` 입력 필드가 반드시 채워져야 하는지 여부를 나타냅니다.
- `readonly` 입력 필드를 읽기 전용으로 만듭니다. 즉, 사용자가 값을 변경할 수 없습니다.
- `disabled` 입력 필드를 비활성화합니다. 사용자가 값을 입력할 수 없습니다.
</details>

<details>
<summary>input type에는 어떤 것이 있나요? (10.6)</summary>
<br />

- `text` 텍스트 입력
- `email` 이메일 입력
- `password` 비밀번호 입력
- `date` 날짜 입력
- `number` 숫자 입력
  - `min`, `max`, `step` attribute를 사용하여 입력 가능한 값의 범위와 증가 단위를 지정할 수 있습니다.
- `range` 슬라이더 형태의 입력
- `checkbox` 체크박스
  - `name`의 값이 `on`, `off`라는 문자열로 지정됩니다.
  - `value` 속성을 써서 `name`의 값을 `value` 속성값(문자열)로 지정할 수 있습니다.
- `radio` 라디오 버튼
  - checkbox와 비슷하지만 여러 항목 중 하나의 항목만 선택할 수 있습니다.
- `file` 파일 업로드
  - `accept` attribute를 써서 허용할 파일 확장자들을 정할 수 있습니다.
  - `multiple` attribute를 써서 여러 개의 파일을 선택할 수 있게 할 수 있습니다.
- `submit` 서버로 폼 데이터 전송
</details>

<details>
<summary>&ltbutton&gt 태그의 type 속성값은 어떤 것이 있나요? (3)</summary>
<br />

- `submit` 폼 데이터를 서버로 제출합니다. 이 버튼이 클릭되면 `<form>` 요소에서 action 속성에 지정된 URL로 데이터가 전송됩니다.
  - default event로 url에 qurey string으로 input의 name=value 값을 전달합니다.
- `reset` 폼 데이터를 초기화합니다. 이 버튼이 클릭되면 모든 폼 필드의 값을 초기 값으로 되돌립니다.
- `button` 일반 버튼을 생성합니다. 이 버튼을 클릭해도 아무 일도 발생하지 않습니다. 이 속성을 사용하여 자바스크립트 이벤트 핸들러를 버튼에 연결할 수 있습니다.
</details>

<details>
<summary>다른 form element는 어떤 것이 있나요? (2.7.6)</summary>
<br />

- `<select>`
  - 옵션 목록을 제공하며, 사용자가 목록에서 값을 선택할 수 있도록 합니다.
  - 이 요소는 다음과 같은 속성을 가질 수 있습니다
    - `name` 요소의 이름(Name)을 지정합니다. 폼 데이터의 이름으로 사용됩니다.
		- `multiple` 여러 옵션을 선택할 수 있도록 합니다.
		- `size` 목록에서 표시되는 옵션의 수를 지정합니다.
  - 내부에 `value` 속성을 갖는 `<option>` 태그를 넣어서 구현합니다.
  - 예시
	```html
	<select name="fruit">
		<option value="apple">사과</option>
		<option value="banana">바나나</option>
		<option value="orange">오렌지</option>
	</select>

	```
- `<textarea>`
  - 여러 줄의 텍스트를 입력할 수 있는 텍스트 영역을 제공합니다.
  - 이 요소는 다음과 같은 속성을 가질 수 있습니다
    - `name` 요소의 이름(Name)을 지정합니다. 폼 데이터의 이름으로 사용됩니다.
		- `rows` 텍스트 영역에 보여지는 줄의 수를 지정합니다.
    - `cols` 텍스트 영역에 보여지는 칸의 수를 지정합니다.
  - 예시
	```html
	<textarea name="message" rows="4" cols="40">
		여러 줄의 텍스트를 입력할 수 있습니다.
	</textarea>
	```
</details>

<details>
<summary>link 태그란? (4.4)</summary>
<br />

- HTML 문서에서 다른 문서와의 연결(link)을 지정하는 데 사용됩니다.
- 보통 스타일 시트, 아이콘, 웹 폰트 등의 외부 리소스와의 연결을 지정하는 데 사용됩니다.
- 이 요소는 다음과 같은 속성을 가질 수 있습니다
  - `href` 연결할 문서의 URL을 지정합니다.
  - `rel` 현재 문서와 연결된 문서와의 관계(Relationship)를 지정합니다. 일반적으로 스타일 시트를 연결할 때는 "stylesheet" 값을 사용합니다.
  - `type` 연결된 문서의 MIME 타입을 지정합니다. 스타일 시트를 연결할 때는 "text/css" 값을 사용합니다.
  - `media` 연결된 문서가 적용될 미디어 타입(Media Type)을 지정합니다. 기본값은 "all" 입니다.
- 예시
  ```html
  <head>
    <link rel="stylesheet" type="text/css" href="style.css">
    <link rel="stylesheet" type="text/css" href="fonts.css">
    <link rel="icon" type="image/png" href="favicon.png">
  </head>
  ```
</details>

<details>
<summary>&ltscript&gt 태그란? (2)</summary>
<br />

- script 태그는 HTML 문서에 스크립트를 삽입하는 데 사용됩니다.
- script는 보통 클라이언트 측에서 실행되며, 동적인 기능을 추가하거나 웹 페이지의 동작을 제어하는 데 사용됩니다.
</details>

<details>
<summary>&ltscript&gt 태그의 attribute는 어떤 것이 있나요? (2)</summary>
<br />

- `src` 실행할 스크립트 파일의 URL을 지정합니다. 이 속성을 사용하면 `<script>` 요소 내부에 스크립트 코드를 작성하지 않고 외부 스크립트 파일을 불러올 수 있습니다.
- `type` 스크립트 코드의 MIME 타입을 지정합니다. 일반적으로 "text/javascript" 값을 사용합니다. HTML5부터는 이 속성을 생략해도 기본값으로 "text/javascript"가 지정됩니다.
</details>

<details>
<summary>&ltscript&gt 태그를 작성할 때 고려해야할 사항은 무엇인가요? (4)</summary>
<br />

- `<script>`는 종료 태그가 필요합니다.
- `<script>` 요소를 사용하여 작성된 스크립트는 일반적으로 웹 페이지의 렌더링이 완료된 후 실행됩니다. 따라서, 스크립트에서 HTML 요소를 조작하거나 스타일을 변경하는 등의 작업을 수행하려면 HTML 문서가 모두 로드된 후에 실행되도록 해야 합니다.
- `<script>` 요소를 사용하여 외부 스크립트 파일을 불러올 때는 파일의 URL이 유효한지, 스크립트 파일이 존재하는지 등을 확인해야 합니다.
- 스크립트 파일의 크기가 크거나, 로딩 시간이 길어질 경우 페이지의 로딩 속도가 느려질 수 있습니다. 이러한 경우, 스크립트 파일을 압축하거나, 필요한 경우 비동기적으로 로딩하는 방법을 고려할 수 있습니다.
</details>

<details>
<summary>&ltscript&gt를 &ltbody&gt 태그 내부 마지막에 작성하는 것이 권장되는 이유가 무엇인가요? (2)</summary>
<br />

- 웹 페이지가 로딩되는 동안 스크립트 파일을 다운로드하는 시간이 추가되어 페이지 로딩 속도가 느려질 수 있기 때문입니다.
- 웹 페이지 내용이 전부 렌더링 되기 전에 `<script>` 내부에서 렌더링 되지 않은 DOM 요소에 접근하려 한다면 예기치 못한 오류가 발생할 수 있기 때문입니다.
</details>

<details>
<summary>시맨틱 태그(Semantic tag)란? (3.8)</summary>
<br />

- HTML5에서 소개된 태그 중 하나로, 웹 페이지의 콘텐츠의 의미를 설명하는 역할을 합니다.
- 웹 페이지의 구조와 콘텐츠의 의미를 명확하게 나타낼 수 있어 검색 엔진이나 스크린 리더 등이 웹 페이지를 더 잘 이해하고 처리할 수 있습니다.
- 예시
   - `<header>` 도입부에 해당하는 콘텐츠
   - `<nav>` HTML 문서 사이를 탐색할 수 있는 링크의 집합
   - `<main>` HTML 문서 내에 한 번만 사용할 수 있는 주요 콘텐츠
   - `<footer>` 사이트의 작성자나 저작권 정보, 연락처 등이 있는 콘텐츠
   - `<article>` 독립적인 하나의 콘텐츠
   - `<section>` 전체적인 내용과 관련이 있는 콘텐츠
   - `<aside>` 부가 정보나 광고 등이 있는 콘텐츠
   - `<figure>` image와 image caption이 있는 콘텐츠로 `<figcaption>`을 자식 요소로 쓰곤 합니다.
</details>

<details>
<summary>시맨틱 태그 사용의 이점은 무엇인가요? (5)</summary>
<br />

- 의미 전달의 명확화: Semantic tag는 콘텐츠의 의미와 구조를 명확하게 전달할 수 있습니다. 이는 검색 엔진이나 스크린 리더 등이 웹 페이지를 더 잘 이해하고 처리할 수 있도록 돕습니다.
- 검색 엔진 최적화(Search Engine Optimization, SEO): Semantic tag를 사용하면 검색 엔진이 페이지의 구조와 콘텐츠를 더 잘 인식할 수 있습니다. 따라서 검색 결과에서 상위에 노출될 가능성이 높아집니다.
- 웹 접근성(Web Accessibility = A11y) 향상: Semantic tag를 사용하면 스크린 리더 등의 보조 기술을 사용하는 사용자들도 웹 페이지를 더 쉽게 이해하고 사용할 수 있습니다. 이는 웹 접근성을 높이는 데에 큰 도움이 됩니다.
- 코드 유지 보수성 향상: Semantic tag를 사용하면 코드의 가독성과 유지 보수성이 향상됩니다. 의미 있는 태그를 사용하면 다른 개발자들도 코드를 더 쉽게 이해하고 수정할 수 있습니다.

- 미래 호환성 보장: Semantic tag를 사용하면 새로운 웹 기술이 등장해도 이전에 작성한 코드가 더욱 유연하게 대처할 수 있습니다. Semantic tag를 사용하면 콘텐츠와 구조를 명확하게 전달할 수 있기 때문에, 새로운 기술이 등장해도 이전 코드를 수정하지 않고도 호환성을 유지할 수 있습니다.
</details>
