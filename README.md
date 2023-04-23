## Data Structure




## Algorithm problems




## HTML
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




## CSS
<details>
<summary>CSS란? (9)</summary>
<br>

- CSS(Cascading Style Sheets)는 HTML 및 XML과 같은 마크업 언어로 작성된 문서의 표현 방법을 정의하는 스타일 시트 언어입니다.
- CSS는 웹 사이트 및 웹 응용 프로그램의 디자인 및 레이아웃을 제어하며, HTML과 함께 웹 페이지의 모양과 느낌을 결정하는 데 중요한 역할을 합니다.
- CSS는 문서의 콘텐츠와 디자인을 분리하는 데 중요한 역할을 합니다.
- 이러한 분리는 문서 구조를 더욱 명확하게 하며, 콘텐츠와 디자인 간의 변경을 쉽게 만듭니다.
- CSS를 사용하면 웹 페이지의 색상, 글꼴, 레이아웃 및 다양한 기타 속성을 변경할 수 있습니다.
- CSS는 HTML 요소에 적용되며, 스타일 시트는 HTML 문서 내에 포함됩니다.
- CSS는 다양한 브라우저에서 사용할 수 있습니다.
- CSS는 웹 표준 기술이며, W3C(World Wide Web Consortium)에서 정의하고 유지 관리됩니다.
- 이것은 브라우저 제조사들이 웹 표준을 준수하고 CSS를 지원함으로써 일관된 웹 페이지 디자인과 레이아웃을 보장할 수 있게 해줍니다.
</details>

<details>
<summary>CSS 버전의 역사 (6)</summary>
<br>

- CSS Level 1(1996)
	- 이 버전은 웹 표준화 기구인 W3C(World Wide Web Consortium)에 의해 발표된 CSS의 첫 번째 공식 표준입니다.
- CSS Level 2(1998)
	- 이 버전에서는 위치, 배경, 텍스트, 폰트, 색상 및 레이아웃과 같은 속성에 대한 새로운 기능과 선택자를 도입했습니다.
- CSS Level 2.1(2004)
	- 이 버전은 CSS Level 2를 개정하고 변경 사항을 통합했습니다.
- CSS Level 3(2011)
	- 이 버전에서는 새로운 모듈과 선택자, 애니메이션, 플렉스박스, 그리드 레이아웃 및 그림자와 같은 새로운 기능을 도입했습니다.
	- 대부분의 웹 사이트는 CSS Level 3을 사용하고 있습니다.
</details>

<details>
<summary>CSS 코드를 작성하는 방법 3가지 (3)</summary>
<br>

1. 내부 스타일 시트 (Internal Style Sheet)
  - HTML 문서 애부에 `<style>` 태그를 사용하여 CSS 코드를 작성하는 방법입니다.
  - 이 방법은 한 페이지 내에서만 스타일을 적용할 수 있습니다.
  - 예시
    ```html
    <!DOCTYPE html>
    <html>
    <head>
        <title>내부 스타일 시트 예제</title>
        <style>
            body {
                background-color: #f0f0f0;
                font-family: Arial, sans-serif;
                font-size: 16px;
            }

            h1 {
                color: #333;
                font-size: 24px;
                text-align: center;
                margin-top: 50px;
            }
        </style>
    </head>
    <body>
        <h1>내부 스타일 시트 예제</h1>
        <p>내부 스타일 시트를 사용하여 스타일을 적용한 예제입니다.</p>
    </body>
    </html>
    ```
2. 외부 스타일 시트 (External Style Sheet)
	- CSS 코드를 별도의 파일로 분리하여 HTML 문서에서 불러오는 방법입니다.
  - 이 방법은 여러 페이지에서 동일한 스타일을 적용할 수 있으며, 유지보수와 코드 관리를 용이하게 할 수 있습니다.
  - 예시
    ```html
      <!DOCTYPE html>
      <html>
      <head>
          <title>외부 스타일 시트 예제</title>
          <link rel="stylesheet" type="text/css" href="style.css">
      </head>
      <body>
          <h1>외부 스타일 시트 예제</h1>
          <p>외부 스타일 시트를 사용하여 스타일을 적용한 예제입니다.</p>
      </body>
      </html>
      ```
3. 인라인 스타일 (Inline Style)
	- HTML 태그 내부에서 style 속성을 사용하여 CSS 스타일을 적용하는 방법입니다.
  - 이 방법은 특정 요소에 대해서만 스타일을 적용하고, 다른 방법에 비해 코드가 지저분해질 수 있다는 단점이 있습니다.
  - 예시
    ```html
    <!DOCTYPE html>
    <html>
    <head>
        <title>인라인 스타일 예제</title>
    </head>
    <body>
        <h1 style="color: #333; font-size: 24px; text-align: center; margin-top: 50px;">인라인 스타일 예제</h1>
        <p style="font-family: Arial, sans-serif; font-size: 16px;">인라인 스타일을 사용하여 스타일을 적용한 예제입니다.</p>
    </body>
    </html>
    ```
</details>

<details>
<summary>CSS 속성(CSS Property)은 어떤 것들이 있나요?</summary>
<br>

- [CSS reference - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference) 참조
</details>

<details>
<summary>CSS에서 사용하는 percentage(%)는 어떤 의미인가요? (5)</summary>
<br>

- 백분율 값을 나타내는 CSS 자료형입니다.
- 보통 부모 객체의 width와의 상대적 크기를 지정합니다.
- width, height, margin, padding, font-size처럼 다양한 속성에서 쓸 수 있습니다.
- 예시
  ```html
  <div style="background-color:navy;">
    <div style="width:50%; background-color: black;">
      <div style="width:50%; margin-left:20%; background-color:chartreuse;">
        Width: 25%, Left margin: 10%
      </div>
      <div style="width:30%; margin-right:60%; background-color:pink;">
        Width: 15%, Left margin: 30%
      </div>
    </div>
  </div>
  ```
- margin-left(right) 값에 백분율을 쓰더라도 부모 객체의 width를 기준으로 한다는 것을 알 수 있습니다.
</details>

<details>
<summary>CSS에서 사용하는 auto는 어떤 의미인가요? (5)</summary>
<br>
  
- 해당 요소의 크기나 위치를 자동으로 설정하도록 지정합니다. 이는 일반적으로 브라우저가 자동으로 계산하도록 하거나, 다른 속성 값에 따라 크기나 위치를 결정할 때 사용됩니다.
- `margin: auto;` 해당 요소의 마진을 자동으로 설정하며, 브라우저는 해당 요소의 위치를 계산하여 수평 방향으로만 중앙에 위치시키도록 합니다.
- `width: auto; height: auto;` 내용물(자식 요소)의 크기에 맞춰 해당 요소의 너비나 높이를 자동으로 조절합니다.
  - **예외**: block 요소의 `width: auto`는 `width: 100%`에서 좌우 마진을 뺀 값이 됩니다.
  - **주의**: 부모 객체가 height: auto일 경우 top, bottom 속성을 이용할 수 없고, transform을 이용하여 세로 방향으로 움직여야합니다.
</details>

<details>
<summary>CSS 선언(CSS declaration)이란? (2)</summary>
<br>
  
- CSS 문서에서 사용되는 구문입니다.
- 각 선언은 선택자(selector)와 선언부(declaration block)로 구성됩니다.
  - `selector {property: value;}`
</details>

<details>
<summary>id란? (4)</summary>
<br>

- HTML 요소에 대한 고유한 식별자입니다.
- 문서 내에서 단 하나의 요소에만 지정할 수 있습니다.
- 한 요소에 두 개 이상의 id를 지정할 수 없습니다.
- id 앞에 `#` 기호를 붙여 선택자로 사용됩니다.
</details>

<details>
<summary>class란? (4)</summary>
<br>

- HTML 여러 요소에 대한 스타일을 그룹으로 지정할 수 있게 해주는 식별자입니다.
- ID와 달리 여러 요소에 적용될 수 있습니다.
- ID와 달리 각 요소에 대해 다른 클래스를 지정할 수 있습니다.
- class name 앞에 `.` 기호를 붙여 선택자로 사용됩니다.
</details>

<details>
<summary>CSS에서 색상 단위는 어떤 것이 있나요? (7)</summary>
<br>

- 키워드 (Keyword): red, blue, green, black, white 등과 같은 색상 이름을 사용할 수 있습니다.
- 16진수 (Hexadecimal): #을 사용하여 색상을 표현합니다. 예를 들어, #000000은 검정색이며, #FFFFFF은 흰색입니다.
- RGB: red, green, blue의 값으로 색상을 지정합니다. 예를 들어, rgb(255, 0, 0)은 빨간색입니다.
- RGBA: RGB와 같지만, alpha 값을 추가하여 투명도를 지정할 수 있습니다. 예를 들어, rgba(255, 0, 0, 0.5)는 반투명한 빨간색입니다.
- HSL: hue(색상), saturation(채도), lightness(명도)의 값으로 색상을 지정합니다. 예를 들어, hsl(0, 100%, 50%)은 빨간색입니다.
- HSLA: HSL과 같지만, alpha 값을 추가하여 투명도를 지정할 수 있습니다. 예를 들어, hsla(0, 100%, 50%, 0.5)는 반투명한 빨간색입니다.
- var(--color)같이 var()을 통해 사용자가 정의한 변수 이름을 사용할 수 있습니다.
</details>

<details>
<summary>CSS에서 크기 단위는 어떤 것이 있나요? (8)</summary>
<br>

- 픽셀(px) : 절대 크기 단위로, 고정된 크기 값을 지정할 때 사용됩니다.
- 백분율(%) : 상대 크기 단위로, 부모 요소의 크기에 대한 백분율 값을 사용하여 크기를 지정할 때 사용됩니다.
- em : 상대 크기 단위로, 현재 요소에 지정된 font-size 값에 대한 배수 값을 사용하여 크기를 지정할 때 사용됩니다.
- rem : 상대 크기 단위로, 루트 요소(html)에 지정된 font-size 값에 대한 배수 값을 사용하여 크기를 지정할 때 사용됩니다.
- vw, vh : 뷰포트의 너비와 높이를 기준으로 크기를 지정할 때 사용됩니다.
- vmin, vmax : 뷰포트의 너비와 높이 중 작은 값 또는 큰 값에 대한 비율 값을 사용하여 크기를 지정할 때 사용됩니다.
</details>

<details>
<summary>line-height는 어떤 속성인가요? (4)</summary>
<br>

- 텍스트 요소의 줄 간격을 조정하는 데 사용됩니다.
- 기본값은 normal로, 이 경우 브라우저는 글꼴 크기에 따라 줄 간격을 자동으로 조정합니다.
- 다른 값으로는 길이 값(px, em 등), 상대 값(%, unitless number), 그리고 숫자 값이 있습니다. 숫자 값은 글꼴 크기에 대한 배수를 나타냅니다.
</details>

<details>
<summary>요소의 배경 이미지는 어떻게 다루나요? (4)</summary>
<br>

- `background-image`
  - 요소의 배경 이미지를 설정합니다.
  - 이미지는 URL 또는 linear-gradient()와 같은 CSS gradient 함수로 지정할 수 있습니다.
  - 여러 개의 이미지를 사용할 경우 쉼표(,)로 구분하여 지정할 수 있습니다.
- `background-repeat`
  - 배경 이미지가 반복되는 방식을 지정합니다.
  - repeat(기본값), repeat-x, repeat-y, no-repeat 등의 값으로 설정할 수 있습니다.
- `background-position`
  - 배경 이미지가 위치하는 위치를 지정합니다.
  - top, bottom, left, right, center 등의 값으로 설정하거나, x y 형식으로 좌표값을 직접 지정할 수 있습니다.
- `background-size`
  - 배경 이미지의 크기를 지정합니다.
  - auto(기본값), contain, cover, 50% 50%와 같은 값으로 설정할 수 있으며, width height 형식으로 크기를 직접 지정할 수도 있습니다.
</details>

<details>
<summary>linear-gradient()란? (6)</summary>
<br>

- 배경 그라데이션(gradient)을 생성하기 위한 함수 중 하나로, 시작 색상과 끝 색상을 지정하여 그 사이에 일정한 색상 변화를 만들어냅니다.
- `linear-gradient([<angle> | to <side-or-corner>], <color-stop-list>)`
- `<angle>`은 그라데이션의 각도를 지정합니다.
- `<side-or-corner>`은 그라데이션의 방향을 지정하는 키워드입니다. to right 또는 to left top과 같은 방향도 지정할 수 있습니다.
- `<color-stop-list>`는 그라데이션의 색상과 위치를 지정하는 리스트입니다. 각각의 색상은 CSS 색상값으로 지정하며, 위치는 0~100% 사이의 값을 가집니다. 여러 개의 색상과 위치를 지정할 경우 쉼표(,)로 구분하여 지정할 수 있습니다.
- 예시
  - `background: linear-gradient(to bottom, red, yellow, green);`
  - 위의 코드에서, linear-gradient() 함수는 to bottom 방향으로 그라데이션을 설정하고 있습니다. red, yellow, green 순서로 색상을 지정하였고, 위치는 각각 0%, 50%, 100%로 지정되었습니다. 따라서 .box 요소의 배경은 빨간색에서 노란색으로, 그리고 초록색으로 일정한 색상 변화를 보일 것입니다.
</details>

<details>
<summary>box-shadow란? (3)</summary>
<br>

- 요소의 그림자 효과를 지정할 때 사용됩니다.
- box-shadow 속성의 값은 다음과 같이 지정됩니다.
  - `box-shadow: h-shadow v-shadow blur spread color inset;`
  - `h-shadow` 그림자의 가로 위치
  - `v-shadow` 세로 위치
  - `blur` 흐림 정도
  - `spread` 그림자의 크기
  - `color` 그림자 색상
  - `inset` 그림자가 요소 안쪽에 위치하는지 외부에 위치하는지 여부
- 예시
  - `box-shadow: 2px 2px 4px #888888;`
  - 위 코드에서 요소에 왼쪽으로 2px, 아래쪽으로 2px 이동한 위치에 흐린 정도가 4px이고, 색상이 #888888인 그림자 효과를 추가한다는 뜻입니다.
</details>

<details>
<summary>opacity란? (2)</summary>
<br>

- CSS 속성 중 하나로, 해당 요소의 투명도를 지정하는 데 사용됩니다.
- opacity 속성은 0부터 1 사이의 값을 가지며, 값이 작을수록 요소가 불투명해지고, 값이 클수록 요소가 투명해집니다.
</details>

<details>
<summary>박스 모델(Box model)이란? ()</summary>
<br>

- CSS에서 요소가 차지하는 공간을 나타내는 모델입니다.
- 각각의 요소는 콘텐츠 영역, 패딩 영역, 테두리 영역, 그리고 마진 영역으로 구성되며, 이러한 영역들이 모두 합쳐져서 요소가 차지하는 전체 공간을 형성합니다.
- Box-model을 구성하는 영역들과 관련된 용어
  - 콘텐츠 영역 (Content area): 텍스트, 이미지 등 요소가 실제로 표시되는 부분입니다.
  - 패딩 영역 (Padding area): 콘텐츠 영역 주위의 여백을 말하며, 패딩 값이 있을 경우 해당 요소의 내부 여백을 설정합니다.
  - 테두리 영역 (Border area): 콘텐츠 영역과 패딩 영역 사이의 경계선을 말하며, 테두리 스타일, 두께, 색상 등을 설정할 수 있습니다.
  - 마진 영역 (Margin area): 테두리 영역 주위의 여백을 말하며, 마진 값이 있을 경우 해당 요소의 외부 여백을 설정합니다.
</details>

<details>
<summary>padding과 margin 표기법을 설명해주세요 (5)</summary>
<br>

- `margin: [size]` 상하좌우
- `margin: [size] [size]` 상하/좌우
- `margin: [size] [size] [size]` 상/좌우/하
- `margin: [size] [size] [size] [size]` 상/우/하/좌
- `width: [size]; margin: [size] auto` 자동으로 채우기
  - 너비가 정해져 있어야 자동으로 채울 수 있다.
</details>

<details>
<summary>padding과 margin 표기법을 설명해주세요 (5)</summary>
<br>

- `margin: [size]` 상하좌우
- `margin: [size] [size]` 상하/좌우
- `margin: [size] [size] [size]` 상/좌우/하
- `margin: [size] [size] [size] [size]` 상/우/하/좌
- `width: [size]; margin: [size] auto` 자동으로 채우기
  - 너비가 정해져 있어야 자동으로 채울 수 있다.
</details>

<details>
<summary>border와 border-radius 표기법을 설명해주세요 ()</summary>
<br>

```css
/* 모든 속성 값 지정 */
border: border-width border-style border-color;

/* 속성 값 미지정 */
border: none;
```
```css
/* 모든 모서리를 동일한 값으로 지정 */
border-radius: 10px;

/* 상단 모서리와 하단 모서리를 다르게 지정 */
border-radius: 10px 20px;

/* 상단 왼쪽 모서리, 상단 오른쪽 모서리, 하단 오른쪽 모서리, 하단 왼쪽 모서리를 각각 다르게 지정 */
border-radius: 10px 20px 30px 40px;

/* 모든 모서리에 각각 다른 값을 지정 */
border-radius: 10px 20px 30px 40px / 50px 60px 70px 80px;

/* 요소를 원형으로 만드는 방법 */
border-radius: 50%;
```
</details>

<details>
<summary>box-sizing 속성이란? (3)</summary>
<br>

- CSS 속성 중 하나로, 요소의 크기를 계산하는 방법을 지정합니다.
- `box-sizing` 속성은 다음과 같은 값들을 사용할 수 있습니다.
  - `content-box` 기본값으로, 요소의 크기는 콘텐츠 영역의 크기만을 포함합니다. 패딩과 테두리(border)는 요소의 크기에 포함되지 않습니다.
  - `border-box` : 요소의 크기는 콘텐츠 영역, 패딩, 테두리의 크기를 모두 포함합니다. 이 때, 콘텐츠 영역의 크기가 여백과 테두리의 크기를 감소시키는 효과가 있습니다.
- 전체 요소에 대해 `* {box-sizing: border-box;}`를 설정하는 것은 일반적으로 CSS 작성 시 유용하며, 웹 사이트 전체적인 디자인에 일관성을 부여할 수 있습니다.
</details>

<details>
<summary>overflow란? (2)</summary>
<br>

- 요소의 내용이 지정된 크기를 초과할 때 처리 방법을 지정하는 속성입니다.
- 다음과 같은 값 중 하나를 가질 수 있습니다.
  - `visible` 기본값으로, 초과한 부분을 그대로 표시합니다.
  - `hidden` 초과한 부분을 잘라내고, 표시하지 않습니다.
  - `scroll` 초과한 부분에 스크롤바를 표시하여, 스크롤을 이용해서 보여줍니다.
  - `auto` 필요한 경우에만 스크롤바를 표시합니다.
</details>

<details>
<summary>가로 스크롤을 만드는 방법은? (3)</summary>
<br>

- `overflow-x` 속성을 auto로 하여 가로 스크롤바를 표시합니다. 이때, `overflow-y` 속성은 `hidden` 값을 지정하여 세로 스크롤바를 표시하지 않도록 설정해야 합니다.
- `white-space` 속성을 `nowrap` 값으로 설정하여 요소 내의 텍스트가 줄바꿈 없이 한 줄에 표시되도록 합니다. 이때, 요소의 너비를 초과하는 경우 자동으로 가로 스크롤이 생성됩니다.
- 예시
  ```css
  .container {
  overflow-x: auto;
  overflow-y: hidden;
  white-space: nowrap;
  }
  ```
</details>

<details>
<summary>마진 상쇄(margin collapse)란? (4)</summary>
<br>

- 인접한 블록 요소의 마진 값이 병합되는 현상을 말합니다.
- 이 현상은 다음과 같은 상황에서 발생합니다.
  - 인접한 블록 요소의 상/하단 마진 값이 모두 존재할 경우
  - 부모 요소와 첫 번째 자식 요소 또는 마지막 자식 요소 사이의 마진 값이 존재할 경우
- 마진 병합은 다음과 같은 규칙에 따라 처리됩니다.
  - 인접한 블록 요소의 마진 값 중 더 큰 값을 사용합니다.
  - 부모 요소와 첫 번째 자식 요소, 마지막 자식 요소 사이의 마진 값 중 더 큰 값을 사용합니다.
  - 부모 요소와 첫 번째 자식 요소, 마지막 자식 요소 사이에 다른 요소가 존재한다면, 이러한 마진 병합 현상이 발생하지 않습니다.
- 마진 병합은 다음과 같이 해결합니다.
  - 인접한 블록 요소의 상/하단 마진 값을 각각 0으로 설정합니다.
  - 부모 요소와 첫 번째 자식 요소, 마지막 자식 요소 사이에 빈 요소를 추가합니다.
</details>

<details>
<summary>display 속성값은 어떤 것이 있나요? (11)</summary>
<br>

- none
- block
- inline
- inline-block
- table
- table-row
- table-cell
- flex
- grid
- inline-flex
- inline-grid
</details>

<details>
<summary>display: none이란? (2)</summary>
<br>

- 해당 요소는 HTML 문서의 구조에서는 존재하지만, 실제 화면에는 표시되지 않습니다.
- 요소가 차지하는 공간도 없어지므로, 주로 불필요한 요소를 감추거나, JavaScript를 사용하여 동적으로 요소를 추가/제거할 때 유용합니다.
</details>

<details>
<summary>display: block이란? (3)</summary>
<br>

- 해당 요소를 새로운 줄에서 표시하고, 요소의 너비를 부모 요소의 전체 너비로 설정하는 속성입니다.
- 위에서 아래로 배치됩니다.
- 너비와 높이를 지정할 수 있습니다.
</details>

<details>
<summary>display: block인 HTML 태그는 어떤 것이 있나요? (8)</summary>
<br>

- 블록 레벨 컨테이너 요소: `<div>`
- 문단 요소: `<p>`
- 제목 요소: `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`
- 목록 요소: `<ul>`, `<ol>`
- 목록 항목 요소: `<li>`
- 테이블 요소: `<table>`, `<thead>`, `<tbody>`, `<tfoot>`, `<tr>`, `<th>`, `<td>`,
- 폼 요소: `<form>`, `<fieldset>`, `<legend>`, `<input>`, `<select>`, `<option>`, `<textarea>`, `<button>`, `<optgroup>`, `<datalist>`, `<output>`, `<header>`
- HTML5에서 추가된 요소: `<footer>`, `<nav>`, `<aside>`, `<article>`
</details>

<details>
<summary>display: inline이란? (2)</summary>
<br>

- 해당 요소를 새로운 줄이 아닌, 텍스트 흐름 내에서 표시하는 속성입니다.
- 제약 사항
  - 너비와 높이: 요소는 내용물에 맞게 자동으로 너비와 높이가 결정됩니다. 따라서, 너비와 높이를 직접 설정할 수 없습니다.
  - 패딩과 마진: 요소는 수평 방향의 패딩과 마진은 설정할 수 있지만, 수직 방향의 패딩과 마진은 설정할 수 없습니다.
  - 줄바꿈: 요소는 자동으로 줄바꿈이 되지 않습니다. 따라서, 요소가 너무 길어지면 부모 요소를 벗어나게 됩니다.
</details>

<details>
<summary>display: inline인 HTML 태그는 어떤 것이 있나요? (9)</summary>
<br>

- `span` 인라인 레벨 컨테이너 태그
- `a` 하이퍼링크를 생성하는 태그
- `b` 굵은 글씨체로 표시하는 태그
- `img` 이미지를 표시하는 태그(예외적으로 직접 너비와 높이를 설정할 수 있다.)
- `input` 사용자 입력을 받는 폼 요소 태그 (type 속성에 따라 다양한 종류가 있음)
- `label` 폼 요소의 설명을 제공하는 태그
- `select` 드롭다운 형태의 선택 폼 요소 태그
- `textarea` 여러 줄의 텍스트 입력 폼 요소 태그
- `em`, `i`, `strong`, `cite`, `q`, `dfn`, `code`, `var`, `samp`, `kbd`, `sub`, `sup`, `small` 등
</details>

<details>
<summary>display: inline-block이란? (5)</summary>
<br>

- 요소를 문장 내에서 표시하고, 요소의 너비와 높이를 직접 설정 가능하게 해주는 속성입니다.
- 인라인처럼 줄바꿈이 일어나지 않습니다.
- 인라인처럼 컨텐츠의 너비만큼 너비를 차지합니다.
- 블록처럼 세로 여백을 쓸 수 있습니다.
- 블록처럼 너비나 높이를 지정할 수 있습니다.
</details>

<details>
<summary>display: table, talbe-row, table-cell이란? (3)</summary>
<br>

- `table` 테이블 요소를 표시하며, 요소의 너비를 테이블의 전체 너비에 맞게 설정되게 해주는 속성입니다.
- `table-row` 테이블 행 요소를 표시하며, 요소의 너비를 테이블의 전체 너비에 맞게 설정되게 해주는 속성입니다.
- `table-cell 테이블 셀 요소를 표시하며, 요소의 너비와 높이를 직접 설정 가능하게 해주는 속성입니다.
</details>


<details>
<summary>Flexbox란? (3)</summary>
<br>

- Flexbox는 CSS3에서 새롭게 도입된 레이아웃 방식 중 하나로, 요소들을 유연하게 배치할 수 있는 기능을 제공합니다.
- Flexbox는 부모 요소(flex container)와 자식 요소(flex item)로 구성되며, display: flex 속성을 부모 요소에 적용하여 활성화합니다.
- `flex-direction`, `justify-content`, `align-items`, `align-content` 등의 속성을 사용하여 자식 요소들의 배치를 지정합니다.
  - `flex-direction` 요소의 배치 방향을 지정합니다.
  - `justify-content` 요소를 수평 방향으로 정렬합니다.
  - `align-items` 요소를 수직 방향으로 정렬합니다.
  - `align-content` 여러 줄로 된 요소들의 수직 정렬 방법을 지정합니다.
</details>

<details>
<summary>grid란? (2)</summary>
<br>

- 자식 요소를 행(row)과 열(column)로 구성된 그리드 안에 배치할 수 있습니다.
- `grid-template-columns`과 `grid-template-rows` 속성을 사용하여 행과 열의 크기를 정의하고, `grid-template-areas` 속성을 사용하여 각 영역을 이름으로 정의합니다.
</details>

<details>
<summary>선택자 목록(Selector list)란? (1)</summary>
<br>

- CSS에서 하나 이상의 선택자를 콤마로 구분하여 연결한 것
</details>

<details>
<summary>선택자를 붙여쓰면 어떻게 되나요? (1)</summary>
<br>

- 해당하는 모든 선택자를 가진 요소들을 선택한다
</details>

<details>
<summary>자식, 자손 요소를 선택하는 방법은? (2)</summary>
<br>

- 자식 요소: `parent-selector > child-selector`
- 자손 요소: `parent-selector descendant-selector`
</details>

<details>
<summary>가상 클래스(Pseudo class)란? (1)</summary>
<br>

- 선택자의 특정 상태를 정의하는 데 사용되는 클래스
</details>

<details>
<summary>가상 클래스에 어떤 것들이 있나요? (18)</summary>
<br>

- `:link` 링크에 연결된 페이지를 방문하지 않은 상태
- `:visited` 링크에 연결된 페이지를 방문한 상태
- `:hover` 마우스 커서가 링크 위에 올라가 있는 상태
- `:active` 마우스로 링크를 클릭하고 있는 상태
- `:focus` input 요소에 초점이 맞춰진 상태
- `:checked` input 요소가 체크된 상태
- `:enabled` input 요소가 사용할 수 있는 상태
- `:disabled` input 요소가 사용할 수 없는 상태
- `:required` required 속성을 가진 상태
- `:optional` required 속성을 가지지 않는 상태
- `:first-child` 자식 요소 중 첫 번째 요소
- `:last-child` 자식 요소 중 마지막 요소
- `:nth-child(n)` 자식 요소 중 앞에서부터 n번째에 위치하는 요소
- `:nth-last-child(n)` 자식 요소 중 뒤에서부터 n번째에 위치하는 요소
- `:empty` 아무런 자식 요소도 가지지 않는 상태
- `:root` 문서의 root 요소
- `:not(선택자)` 해당 선택자를 제외한 요소
- `:lang(언어)` 유저의 언어 설정 상태
</details>

<details>
<summary>CSS의 Cascading이란? (2)</summary>
<br>

- 여러 개의 스타일 규칙이 있을 때, 캐스케이드 우선순위에 따라 최종 스타일을 결정하는 과정을 의미합니다.
- 여기서 "cascading"은 "폭포처럼 순서대로 내려가는"이라는 의미로 사용됩니다.
</details>

<details>
<summary>캐스케이드 우선순위(Cascade precedence)를 설명하시오 (4)</summary>
<br>

1. Origin and importance
  - `1-1` CSS transitions
  - `1-2` user-agent (browser) !important
  - `1-3` user !important
  - `1-4` author(developer) !important
  - `1-5` CSS @keyframe animations
  - `1-6` inline style definition(developer)
  - `1-7` author(developer)
  - `1-8` user
  - `1-9` user-agent (browser)
  - `!important`와 `inline style definition`은 스타일 디버깅을 어렵게 만든다.
2. 명시도(Specificity)
  - `2-1` 아이디(IDs)
  - `2-2` 클래스(Classes), 속성(attributes), 가상클래스(pseudo-classes)
  - `2-3` 요소(Elements), 가상요소(pseudo-elements)
3. 상속된 스타일(Inherited style)
  - 부모 태그에 적용된 CSS 규칙은 자손에게도 상속됩니다.
    - 모든 속성이 상속되는 건 아니고, 상속되는 속성(`color`, `font-family`, `font-size`, `font-weight`, `line-height`, `text-align`, ... 등)들이 정해져 있습니다.
    - **[Full property table](https://www.w3.org/TR/CSS21/propidx.html)**,
    **[inheritance - Which CSS properties are inherited? - Stack Overflow](https://stackoverflow.com/questions/5612302/which-css-properties-are-inherited)** 참조
    - 가까운 조상에게 물려받은 속성일수록 우선순위가 높습니다.
4. 코드 상의 순서
  - 동일한 가중치를 갖는 규칙이 두 개 이상인 경우, 코드에서 아래 쪽에 쓴 코드일수록 우선순위가 높습니다.
</details>




## JavaScript




## ReactJS




## Git




## UI/UX




## etc

<details>
<summary>()</summary>
<br>

- 
</details>
