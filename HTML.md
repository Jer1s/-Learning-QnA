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

<details>
<summary>하이퍼링크(Hyperlink)란? (4)</summary>
<br>

- 웹 페이지에서 클릭 가능한 링크를 의미합니다.
- 이 링크는 클릭하면 해당 웹 페이지나 문서, 이미지, 비디오, 음악 파일 등 다른 컨텐츠로 이동할 수 있습니다.
- HTML에서 클릭 가능한 텍스트를 만들기 위해서는 `<a>` 태그를 사용합니다. 
- 예시
  - `<a href="path">`
  - 절대 경로(absolute path) 또는 상대 경로(relative path)로 경로를 표시한다.
</details>

<details>
<summary>&lta&gt 태그의 타겟 속성(target attribute)이란? (6)</summary>
<br>

- target 속성은 링크된 페이지를 어떻게 열지 지정하는 데 사용됩니다.
- `_self` 링크된 페이지를 현재 창 또는 탭에서 엽니다(기본값).
- `_blank` 링크된 페이지를 새 창이나 탭에서 엽니다.
- `_parent` 현재 프레임의 상위 프레임에서 링크된 페이지를 엽니다.
- `_top` 현재 모든 프레임을 새로운 창 또는 탭으로 대체하고, 링크된 페이지를 엽니다.
- `framename` 링크된 페이지가 지정된 이름을 가진 프레임 또는 iframe에 로드됩니다.
  - frame은 검색 엔진 최적화(SEO)에 좋지 않은 영향을 미칠 수 있고, 일부 브라우저에서는 더 이상 지원되지 않을 수 있습니다.
</details>

<details>
<summary>URL이란? (2)</summary>
<br>

- URL(Uniform Resource Locator)은 URI의 한 형태로, 인터넷에서 리소스의 위치를 나타냅니다.
- URL은 scheme, 프로토콜, 호스트명, 포트 번호, 경로, 쿼리를 포함할 수 있습니다.
</details>

<details>
<summary>URI란? (1)</summary>
<br>

- URI(Uniform Resource Identifier)는 인터넷에서 특정한 리소스를 나타내는 유일한 식별자입니다.
</details>

<details>
<summary>URI의 구조는 어떻게 되나요? (6)</summary>
<br>

- `scheme:[//[user:password@]host[:port]][/]path[?query][#fragment]`
  - `URI Scheme`
    - URI를 구분하는 스키마(프로토콜)를 나타냅니다.
    - 예를 들어, `http`, `https`, `ftp`, `mailto`, `tel` 등이 있습니다.
    - IANA의 [URI Scheme list](https://www.iana.org/assignments/uri-schemes/uri-schemes.xhtml) 참조
  - `user:password@`
    - 선택적으로 사용되며, 인증 정보를 나타냅니다.
  - `host`
    - 리소스를 호스팅하는 호스트 이름을 나타냅니다.
    - 예를 들어, `www.example.com`과 같은 도메인 이름을 사용할 수 있습니다.
  - `port`
    - 선택적으로 사용되며, 리소스에 액세스하는 데 사용되는 포트 번호를 나타냅니다.
    - 예를 들어, "80"이나 "443"과 같은 포트 번호를 사용할 수 있습니다.
  - `path`
    - 리소스의 경로를 나타냅니다.
    - 예를 들어, "/index.html"과 같은 경로를 사용할 수 있습니다.
  - `query`
    - 선택적으로 사용되며, 리소스에 대한 추가적인 정보를 전달하는 데 사용됩니다.
    - 예를 들어, "key=value"와 같은 쿼리 문자열을 사용할 수 있습니다.
  - `fragment`
    - 선택적으로 사용되며, 리소스의 특정 부분을 나타내는 앵커를 나타냅니다.
    - 예를 들어, "section1"과 같은 앵커를 사용할 수 있습니다.
</details>

<details>
<summary>Text tag는 어떤 것이 있나요? (11)</summary>
<br>

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
<br>

- `<ol>` 순서 있는 리스트(Ordered List)를 나타냅니다.
- `<ul>` 순서 없는 리스트(Unordered List)를 나타냅니다.
- `<li>` 리스트 항목(List Item)을 나타냅니다.
- `<ol>` type attribute
   - `1`, `a`, `A`, `i`, `I` 등
- `<ul>` type attribute
   - `disc`, `circle`, `square` 등
- `<ol>`, `<ul>`에 `list-style` property를 활용할 수 있다.
  - `list-style: list-style-type list-style-position list-style-image`
</details>

<details>
<summary>table tag에 대해 설멍해주세요. (9)</summary>
<br>

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
<summary>&lttable&gt에 사용할 수 있는 border 관련 속성(property) 두 가지는 무엇인가요? (2)</summary>
<br>

- `border-collapse` 인접한 셀의 경계선을 병합할 것인지 여부를 결정합니다. 
  - `collapse` 인접한 셀의 경계선을 병합합니다. 이때 인접한 셀들의 경계선이 중복되지 않습니다. (기본값)
  - `separate` 인접한 셀의 경계선을 병합하지 않습니다. 이때 인접한 셀들의 경계선이 중복됩니다.
- `border-spacing` 인접한 셀 간의 간격을 설정합니다.
  - border-collapse 속성의 값이 separate인 경우에만 적용됩니다.
  - 이 속성의 값은 길이 또는 백분율로 지정할 수 있습니다.
</details>

<details>
<summary>img 태그란? (6)</summary>
<br>

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
<br>

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
<br>

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
<br>

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
<summary> ()</summary>
<br>

- 
</details>


<details>
<summary> ()</summary>
<br>

- 
</details>


<details>
<summary> ()</summary>
<br>

- 
</details>


<details>
<summary> ()</summary>
<br>

- 
</details>


<details>
<summary> ()</summary>
<br>

- 
</details>


<details>
<summary> ()</summary>
<br>

- 
</details>



