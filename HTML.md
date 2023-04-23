<details>
<summary>HTML이란? (4)</summary>
<br>

- HTML은 HyperText Markup Language의 약자이며 웹 페이지 및 기타 온라인 콘텐츠를 만드는 데 사용되는 표준 마크업 언어입니다.
- HTML은 웹 개발자가 콘텐츠를 구성하고 웹 브라우저에서 사용자에게 콘텐츠를 표시하는 방법을 제공합니다.
- 웹 페이지 내용, 레이아웃 및 스타일을 정의하는 다양한 HTML 태그 및 속성을 사용하여 이 작업을 수행할 수 있습니다.
- HTML은 World Wide Web의 초석 기술이며 일반적으로 CSS(Cascading Style Sheet) 및 JavaScript와 같은 다른 웹 기술과 함께 사용됩니다.
</details>

<details>
<summary>하이퍼텍스트(HyperText)란? (4)</summary>
<br>

- 하이퍼텍스트는 다른 텍스트에 대한 링크가 포함된 텍스트를 가리키며, 해당 링크를 클릭하거나 눌러 액세스할 수 있습니다.
- 하이퍼텍스트의 개념은 사용자가 하이퍼링크를 클릭하여 다른 페이지와 문서를 탐색할 수 있는 World Wide Web에 필수적입니다.
- 하이퍼텍스트는 독자가 다른 섹션이나 관련 내용으로 이동할 수 있는 비선형 문서를 작성하는 데 사용되며, 보다 상호 작용적이고 동적인 읽기 환경을 제공합니다.
- 하이퍼텍스트는 종종 HTML과 같은 마크업 언어와 연결되어 개발자가 웹 페이지와 다른 온라인 콘텐츠 사이에 링크를 만들 수 있습니다.
</details>

<details>
<summary>마크업 언어(Markup language)란? (5)</summary>
<br>

- 마크업 언어는 컴퓨터에서 문서의 구조와 포맷을 지정하기 위해 사용되는 언어입니다.
- 마크업 언어는 특수한 코드를 사용하여 문서의 텍스트, 이미지, 비디오 등과 같은 콘텐츠의 표시 방법을 지정합니다.
- 마크업 언어는 일반 텍스트와 구별되도록 특수한 태그나 괄호, 기호 등을 사용하여 표현됩니다.
- 마크업 언어는 문서의 구조와 포맷을 더욱 명확하게 정의하여, 문서의 가독성을 향상시키고 다른 시스템 간에 문서를 쉽게 공유할 수 있도록 합니다.
- HTML,XML, SGML, Markdown, LaTeX 등의 다양한 마크업 언어가 있으며, 각각 다른 목적으로 사용됩니다.
</details>

<details>
<summary>HTML 버전의 역사 (6)</summary>
<br>

- HTML(1991)
- HTML 2.0(1995)
  - HTML의 첫 표준화 버전입니다.
  - 테이블과 이미지 링크 등의 새로운 기능을 도입했습니다.
- HTML 3.2(1997)
  - 인라인 스타일, 폼 등의 새로운 태그를 도입했습니다.
- HTML 4.0(1998)
  - 프레임, 스타일 시트, 자바스크립트 등의 새로운 기능을 도입했습니다.
- XHTML 1.0(2000)
  - HTML을 XML의 엄격한 문법에 따라 작성된 버전입니다.
- HTML5(2014)
  - 웹 페이지를 더욱 인터랙티브하게 만들 수 있는 새로운 기능과 태그를 도입했습니다.
  - 비디오, 오디오, 캔버스, 지리 정보 등을 포함하는 다양한 콘텐츠를 쉽게 표시할 수 있습니다.
  - 현재, 가장 널리 사용되는 HTML 버전입니다.
  - 브라우저 제조사와 W3C(World Wide Web Consortium)는 HTML5를 지원하며, HTML5를 사용하여 더욱 풍부하고 혁신적인 웹 경험을 제공할 수 있습니다.
</details>

<details>
<summary>일부 웹 브라우저에서 HTML 문서의 한글 텍스트가 깨지는 이유 (3)</summary>
<br>

- 일부 웹 브라우저에서 인코딩을 제대로 인식하지 못하거나, 다른 인코딩을 사용하는 경우에 한글 문자를 올바르게 해석하지 못해서 깨진 문자로 표시됩니다.
- HTML 문서는 일반적으로 UTF-8 또는 다른 문자 인코딩을 사용하여 저장됩니다.
- 이 인코딩은 HTML 문서 내의 문자를 컴퓨터가 이해할 수 있는 바이너리 코드로 변환하는 데 사용됩니다.
</details>

<details>
<summary>위 문제의 해결하시오 (1)</summary>
<br>

- HTML 문서의 head 섹션에 charset 속성을 추가하여 문서의 문자 인코딩을 명시적으로 설정할 수 있습니다.
  ```html
  <head>
    <meta charset="UTF-8">
    <title>문서 제목</title>
  </head>
  ```
</details>

<details>
<summary>웹 브라우저 인코딩(Web Browser Encoding)이란? (5)</summary>
<br>

- 웹 브라우저 인코딩(Web Browser Encoding)은 웹 브라우저가 인터넷 상에서 전송되는 텍스트 데이터를 해석하는 방법을 지정하는 것을 말합니다.
- 인코딩은 문자 집합(Character Set)을 바이트로 변환하는 과정입니다. 문자 집합은 컴퓨터에서 표현 가능한 문자들의 집합이며, 각 문자는 고유한 코드 값으로 표현됩니다. 예를 들어, 한글은 유니코드(Unicode)에서 U+AC00부터 U+D7AF까지의 코드 범위에 해당하는 코드 값을 가집니다.
- 웹 페이지는 보통 HTML, CSS, JavaScript 등의 텍스트 데이터로 이루어져 있습니다. 이러한 텍스트 데이터는 문자 집합을 기반으로 작성되며, 웹 브라우저는 이를 해석하여 사용자에게 표시합니다.
- 웹 브라우저 인코딩은 웹 페이지의 텍스트 데이터를 바이트로 변환하는 데 사용되는 인코딩 방식을 지정합니다. 대부분의 웹 브라우저는 UTF-8 인코딩을 기본값으로 사용합니다. UTF-8은 전 세계 대부분의 문자를 표현할 수 있는 유니코드 인코딩 방식 중 하나이며, 인터넷에서 광범위하게 사용됩니다.
- 하지만 때로는 웹 페이지에 다른 인코딩 방식을 사용하는 경우도 있습니다. 이 경우, 사용자는 웹 브라우저의 인코딩 설정을 변경하여 해당 인코딩 방식으로 웹 페이지를 해석할 수 있습니다.
</details>

<details>
<summary>UTF-8이란? (4)</summary>
<br>

- UTF-8은 컴퓨팅 시스템에서 텍스트를 표현하는 데에 널리 사용되는 문자 인코딩 표준입니다.
- 가변 길이 인코딩 방식으로, 각 문자는 해당하는 유니코드 코드 포인트에 따라 1바이트에서 4바이트까지 표현될 수 있습니다.
- UTF-8은 ASCII와 하위 호환성을 가지도록 설계되어 있습니다. 즉, 첫 128개 코드 포인트(ASCII 문자에 해당하는 부분)는 한 바이트로 표현됩니다. 이로 인해 주로 ASCII 문자를 사용하는 언어의 텍스트 처리에 매우 효율적이며, 다른 문자 체계와 언어의 문자를 표현할 수 있는 유연성도 제공합니다.
- UTF-8은 현재 웹에서 우위를 점하고 있으며, 거의 모든 최신 웹 브라우저와 운영 체제에서 지원됩니다. 또한 프로그래밍 언어와 데이터베이스 시스템에서도 널리 사용됩니다.
</details>

<details>
<summary>HTML 파일의 기본 구조를 설명하시오 (1)</summary>
<br>

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
<summary>&lt&#33DOCTYPE html&gt란? (6)</summary>
<br>

- <\!DOCTYPE html>은 HTML5 문서 유형 선언(doctype declaration)입니다.
- 이 선언은 HTML5에서 문서가 사용하는 버전을 명시하는 역할을 합니다.
- 명시적으로 선언하지 않으면 브라우저가 페이지를 렌더링할 때 자동으로 quirks mode로 동작할 수 있으므로 <\!DOCTYPE html>을 사용하여 명시적으로 문서 유형을 선언하는 것이 좋습니다.
- <\!DOCTYPE html>은 HTML5 문서에서 항상 사용되는 유일한 선언입니다.
- <\!DOCTYPE html>을 문서의 가장 위에 위치시키는 것이 좋습니다.
- 이전 버전의 HTML에서는 문서 유형 선언이 더 긴 형식으로 작성되었습니다.
</details>

<details>
<summary>태그(Tag)란? (2)</summary>
<br>

- HTML에서 태그는 꺾쇠 기호(angle bracket)를 사용하는 문법입니다.
- 일반적으로 시작 태그와 종료 태그로 내용을 감쌉니다.
</details>

<details>
<summary>단일 태그(single tag)란? (4)</summary>
<br>

- 종료 태그가 필요하지 않습니다.
- 예시
  - `<br>` 줄 바꿈 태그
  - `<img>` 이미지 태그
  - `<input>` 입력 필드 태그
  - `<meta>` 문서 정보 태그
  - `<link>` 외부 리소스 연결 태그
  - `<hr>` 수평선 태그
- 빈 요소(empty element)라고도 부릅니다.
- 태그 마지막에 슬래시(/) 기호를 넣어서 단일 태그라는 표시를 할 수도 있습니다. (이전 버전의 HTML 문법입니다.)
</details>

<details>
<summary>태그 속성(attribute)란? (6)</summary>
<br>

- HTML 태그에 추가 정보를 제공하는 데 사용됩니다.
- 속성은 일반적으로 "속성명(attribute name)=속성값(attribute value)"의 형식으로 작성됩니다.
- 속성은 대소문자를 구분하지 않으며, 보통 소문자로 작성됩니다.
- 예시
  - `class` 요소에 대한 CSS 클래스 이름을 지정합니다.
  - `id` 요소의 고유한 식별자를 지정합니다.
  - `style` 요소에 대한 인라인 CSS 스타일을 지정합니다.
  - `title` 요소에 대한 추가 정보(툴팁)를 제공합니다.
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
<summary>사용자 정의 속성(Custom attribute)이란? (5)</summary>
<br>

- 사용자 정의 속성은 HTML 요소에 사용자가 원하는 속성을 추가할 수 있는 방법입니다.
- 사용자 정의 속성은 `data-*` 형식으로 정의됩니다. 여기서 `*` 부분은 사용자가 원하는 이름을 사용할 수 있습니다.
- `data-`를 붙이지 않아도 작동하지만, 사용자 정의 속성이 표준 속성으로 편입될 경우 예기치 못한 오류를 발생시킬 수 있기 때문에 data-를 붙이는 것이 좋습니다.
- W3C에서 규정한 HTML 규약에 따라 작성되어야 합니다.
- 모든 브라우저가 사용자 정의 속성을 지원하는 것은 아니므로, 브라우저 호환성에 주의해야 합니다.
</details>

<details>
<summary>HTML tags는 어떤 것들이 있나요?</summary>
<br>

- [HTML elements reference - HTML: HyperText Markup Language | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element) 참조
</details>

<details>
<summary>&ltmeta http-equiv="X-UA-Compatible" content="IE=edge, chrome=1"&gt가 의미하는 바는 무엇인가요? (5)</summary>
<br>

- 웹 페이지를 렌더링하는 데 사용되는 인터넷 익스플로러(IE) 버전을 지정하는 데 사용됩니다.
- `http-equiv` 사용할 HTTP 응답 헤더를 지정합니다.
- `content` IE 버전을 지정합니다. 
  - `edge` 브라우저가 사용자의 컴퓨터에 설치된 최신 IE 버전을 사용하도록 지시합니다.
  - `chrome=1` Google Chrome Frame이 설치된 경우 해당 플러그인을 사용하여 웹 페이지를 렌더링하도록 합니다.
</details>

<details>
<summary>&ltmeta name="viewport" content="width=device-width, initial-scale=1.0"&gt가 의미하는 바는 무엇인가요? (5)</summary>
<br>

- 이 메타 태그는 웹 페이지의 뷰포트(viewport)를 정의하여 다른 기기에서 웹 페이지가 어떻게 표시되는지 제어합니다.
- 모바일 기기에서 웹 페이지가 다른 화면 크기에서 올바르게 표시되도록 하는 데 특히 중요합니다.
- `name` 메타데이터 유형을 지정합니다.
- `content` 해당 메타데이터의 값을 지정합니다.
  - `width=device-width` 뷰포트의 너비를 기기의 너비로 설정합니다.
  - `initial-scale=1.0` 초기 줌 레벨을 1.0으로 설정합니다.
</details>

<details>
<summary>메타 태그(Meta tag)란? (4)</summary>
<br>

- 메타 태그(meta tag)는 HTML 문서의 `<head>` 태그 내에 작성되는 태그로, 웹 페이지의 메타데이터(meta data)를 정의하는 데 사용됩니다.
- 메타데이터는 문서에 대한 부가 정보를 제공하는 데이터를 의미합니다. 예를 들어, 웹 페이지의 제목(title), 설명(description), 작성자(author), 키워드(keywords), 문자 인코딩(charset) 등이 메타데이터에 해당합니다.
- 메타 태그는 검색 엔진 최적화(SEO)를 위해 사용될 수도 있습니다. 검색 엔진은 메타 태그를 분석하여 웹 페이지의 내용과 일치하는 검색어를 찾아 검색 결과에 반영합니다.
- 예시
  - `<meta name="description" content="웹 페이지 설명">` 웹 페이지의 설명을 나타내는 메타 태그입니다.
  - `<meta http-equiv="refresh" content="5;url=https://example.com">` 5초 후에 `https://example.com`로 이동하는 메타 태그입니다.
</details>

<details>
<summary>오픈그래프(Open Graph)란? (4)</summary>
<br>

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
<br>

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
<summary>구글 애널리틱스(Google Analytics란? (4)</summary>
<br>

- 구글이 제공하는 웹 분석 도구로, 웹 사이트 방문자들의 행동 및 트래픽을 추적하고 분석하여 웹 사이트의 성과를 파악할 수 있도록 도와줍니다.
- Google Analytics를 사용하면 웹 사이트 방문자들의 정보를 수집하고, 이를 분석하여 사용자가 웹 사이트에서 어떤 행동을 하는지, 어디서 왔는지, 어떤 장치나 브라우저를 사용하는지 등을 파악할 수 있습니다. 이를 통해 웹 사이트의 성과를 평가하고, 사용자 경험을 개선하거나 마케팅 전략을 수립할 수 있습니다.
</details>
