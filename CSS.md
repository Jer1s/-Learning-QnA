<details>
<summary>CSS란?(6)</summary>
<br />

- CSS(Cascading Style Sheets)는 HTML 및 XML과 같은 마크업 언어로 작성된 문서의 스타일을 정의하는 스타일시트 언어입니다.
- CSS는 웹 페이지의 배경색, 폰트, 레이아웃, 애니메이션 등 다양한 디자인 및 레이아웃 속성을 제어하여 웹 페이지의 모양과 느낌을 결정하는 중요한 역할을 합니다.
- CSS의 주요 이점 중 하나는 웹 페이지의 구조(HTML 또는 XML)와 표현(CSS)을 분리하는 것입니다. 이로 인해 웹 개발자는 내용을 변경하지 않고 디자인을 수정하거나, 반대로 디자인을 변경하지 않고 내용을 업데이트할 수 있습니다. 이는 웹 페이지의 유지 관리를 쉽게 만들고 웹 페이지의 접근성을 향상시킵니다.
- CSS는 웹 페이지를 만들 때 웹 표준 기술 중 하나로, W3C (World Wide Web Consortium)에서 정의하고 유지 관리합니다. 이 표준은 웹 브라우저 제조사들이 일관된 디자인 및 레이아웃을 제공할 수 있도록 하며, 웹 페이지가 다양한 장치 및 화면 크기에서도 일관된 뷰를 제공할 수 있게 합니다.
- CSS는 HTML 요소를 선택하고 해당 요소에 적용할 스타일 규칙을 정의하는 방식으로 작동합니다. 이러한 규칙은 HTML 문서에 직접 삽입하거나 외부 CSS 파일을 참조하는 방식으로 적용할 수 있습니다.
- CSS는 세부적인 스타일 제어가 가능하며, 웹 페이지의 각 요소에 대한 개별적인 스타일 설정이 가능해 높은 디자인 유연성을 제공합니다. 이는 웹 페이지의 전반적인 브랜드 이미지와 일관성을 유지하는 데 도움이 됩니다.
</details>

<details>
<summary>CSS 버전의 역사 (4.9)</summary>
<br />

- CSS Level 1(1996)
  - CSS의 첫 번째 공식 버전으로, W3C(World Wide Web Consortium)에 의해 발표되었습니다.
  - 이 버전은 웹 페이지의 텍스트 속성과 배경색 등 기본적인 스타일링 요소를 제어하는 기능을 제공했습니다.
- CSS Level 2(1998)
  - CSS의 두 번째 버전으로, 위치 지정, z-index, 미디어 타입 등 웹 페이지 디자인에 대한 더욱 고급 기능을 도입했습니다.
  - 선택자의 기능이 확장되어 더욱 다양한 HTML 요소를 대상으로 스타일을 적용할 수 있게 되었습니다.
- CSS Level 2.1(2004)
  - CSS Level 2를 개정하고 업데이트된 버전입니다.
  - 일부 버그 수정과 함께, 이전 버전에서 추가된 기능의 호환성 문제를 해결하기 위한 변경 사항이 포함되었습니다.
- CSS Level 3(2011)
  - CSS Level 3는 여러 모듈로 분리되어 개발되었으며, 각 모듈은 특정 기능에 대한 정의를 제공합니다.
 - 새로운 기능과 선택자가 추가되었고, 애니메이션, 플렉스박스, 그리드 레이아웃, 그림자, 반응형 웹 디자인을 위한 미디어 쿼리 등의 고급 디자인 기능이 도입되었습니다.
  - 웹페이지의 스타일링에 대한 제어력을 크게 향상시켰으며, 현재 웹 개발에 널리 사용되는 버전입니다.
</details>

<details>
<summary>CSS 코드를 작성하는 방법 3가지 (3.10)</summary>
<br />

- 내부 스타일 시트 (Internal Style Sheet)
	- 내부 스타일 시트(Internal Style Sheet)는 HTML 문서 내의 `<style>` 태그를 사용하여 CSS 코드를 작성하는 방법입니다.
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
- 외부 스타일 시트
	- 외부 스타일 시트(External Style Sheet)는 CSS 코드를 별도의 `.css` 파일로 분리하고, HTML 문서에서 이를 불러오는 방법입니다.
	- 외부 스타일 시트를 사용하면 같은 스타일 규칙을 여러 HTML 페이지에 쉽게 적용할 수 있으며, 유지 관리 및 코드 재사용성이 용이합니다.
	- 외부 CSS 파일을 HTML에서 불러올 때는 `<link>` 태그를 사용합니다.
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
- 인라인 스타일
	- 인라인 스타일(Inline Style)은 HTML 요소의 style 속성을 이용하여 직접 CSS 스타일을 적용하는 방법입니다.
	- 이 방법은 간단한 스타일 변경이 필요할 때 유용하나, 스타일 규칙이 많아지거나 여러 요소에 같은 스타일을 적용해야 할 때는 코드가 지저분해지고 유지 관리가 어려워질 수 있습니다.
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
<br />

- [CSS reference - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference) 참조
</details>

<details>
<summary>CSS에서 사용하는 percentage(%)는 어떤 의미인가요? (5)</summary>
<br />

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
<br />
  
- 해당 요소의 크기나 위치를 자동으로 설정하도록 지정합니다. 이는 일반적으로 브라우저가 자동으로 계산하도록 하거나, 다른 속성 값에 따라 크기나 위치를 결정할 때 사용됩니다.
- `margin: auto;` 해당 요소의 마진을 자동으로 설정하며, 브라우저는 해당 요소의 위치를 계산하여 수평 방향으로만 중앙에 위치시키도록 합니다.
- `width: auto; height: auto;` 내용물(자식 요소)의 크기에 맞춰 해당 요소의 너비나 높이를 자동으로 조절합니다.
- **예외**: block 요소의 `width: auto`는 `width: 100%`에서 좌우 마진을 뺀 값이 됩니다.
- **주의**: 부모 객체가 height: auto일 경우 top, bottom 속성을 이용할 수 없고, transform을 이용하여 세로 방향으로 움직여야합니다.
</details>

<details>
<summary>CSS 선언(CSS declaration)이란? (2)</summary>
<br />
  
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
<summary>박스 모델(Box model)이란? (3)</summary>
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
<summary>border와 border-radius 표기법을 설명해주세요 (7)</summary>
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
<summary>display: inline-block이란? (5)</summary>
<br>

- 요소를 문장 내에서 표시하고, 요소의 너비와 높이를 직접 설정 가능하게 해주는 속성입니다.
- 인라인처럼 줄바꿈이 일어나지 않습니다.
- 인라인처럼 컨텐츠의 너비만큼 너비를 차지합니다.
- 블록처럼 세로 여백을 쓸 수 있습니다.
- 블록처럼 너비나 높이를 지정할 수 있습니다.
</details>

<details>
<summary>Flexbox란? (2)</summary>
<br>

- Flexbox는 CSS3에서 새롭게 도입된 레이아웃 방식 중 하나로, 요소들을 유연하게 배치할 수 있는 기능을 제공합니다.
- Flexbox는 부모 요소(flex container)와 자식 요소(flex item)로 구성되며, display: flex 속성을 부모 요소에 적용하여 활성화합니다.
</details>

<details>
<summary>Flexbox 정렬 (6)</summary>
<br>

- Main Axis: 배치 방향
- Cross Axis: 배치 방향에 수직인 방향
- justify-content: main axis 방향으로 콘텐츠 간의 여백 설정
- align-content: cross axis 방향으로 콘텐츠 간의 여백 설정
- align-items: cross axis 방향으로 모든 요소의 위치 결정
- align-self: cross axis 방향으로 한 요소의 위치 결정
- flex-wrap: overflow된 요소의 줄 바꿈 설정
	- wrap
	- no-wrap
	- wrap-reverse
</details>

<details>
<summary>Flexbox 간격</summary>
<br>

- `gap: {row-gap} {column-gap}`
- gap 속성값은 flex-direction의 영향을 받지 않는다.	
</details>

<details>
<summary>Flexbox 요소 꽉 채우기 (5)</summary>
<br>

- flex-grow
	- default: 0
	- 형제 요소들의 flex-grow 값의 비율에 따라 남은 여백을 분배하여 각 요소의 너비/높이를 늘려준다.
	- 1 값을 주면 빈 공간을 채울 수 있다
- flex-shrink
	- default: 1
	- 형제 요소들의 flex-shrink 값의 비율에 따라 overflow가 일어난 너비/높이를 분배하여 각 요소의 너비/높이를 줄여준다.
	- 0 값을 주면 요소를 원하는 위치에 고정할 수 있다
- flex-basis
	- default: auto
	- flex 요소의 기본 사이즈를 지정한다.
	- width와 사용하는 단위가 같다.
	- 기본값인 auto로 지정된 경우 컨텐츠 사이즈에 맞춰서 나타나고, 0px/0% 값을 주면 부모 컨테이너를 기준으로 크기가 정해진다.
- `flex: {flex-grow} {flex-shrink} {flex-basis}` 형태로 쓸 수 있다
- `display: inline-flex`를 활용해 인라인 안에서 플렉스박스를 만들 수 있다
</details>

<details>
<summary>grid란? (2)</summary>
<br>

- 자식 요소를 행(row)과 열(column)로 구성된 2차원 레이아웃 메소드입니다.
</details>

<details>
<summary>grid 나누는 방법 (2)</summary>
<br>

- `grid-template-columns`과 `grid-template-rows` 속성을 사용하여 행과 열의 크기를 정의하고, `grid-template-areas` 속성을 사용하여 각 영역을 이름으로 정의합니다.
	- `grid-template-columns: {width1} {width2} ...`
   	- `grid-template-rows: {height1} {height2} ...`
   	- `grid-template: {height1} {height2} ... / {width1} {width2} ...`
</details>

<details>
<summary>grid 크기와 함수들 (7)</summary>
<br>

- grid-auto-rows/grid-auto-columns 속성으로 row/column 크기를 자동 지정할 수 있다
- grid-row/grid-column 속성값으로 그리드라인의 번호를 입력해 요소를 원하는 셀 집합에 배치할 수 있다
	- span n 속성값도 쓸 수 있다
- grid item에 grid-area라는 이름을 붙이고 grid container에 grid-template-areas 속성을 이용해 이름으로 배치할 수 있다
	- 해당 위치를 비우고 싶으면 마침표(.)를 쓰면 된다
- size에 fr(fraction) 값을 넣으면 요소 간 상대적인 크기로 지정할 수 있다
	- size에 minmax(min, max) 함수를 활용할 수 있다
	- minmax에서 최댓값에만 fr 값을 쓸 수 있다
	- size에 repeat(n, size) 함수를 활용할 수 있다
- `gap: {row-gap} {column-gap}`
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


<details>
<summary>Position property란? (2)</summary>
<br>

- 요소의 포지션 방법을 명시하는 속성입니다.
- top, right, bottom, left, inset 속성으로 구체적인 위치를 지정할 수 있습니다.
</details>


<details>
<summary>Position property의 종류 (5)</summary>
<br>

- static(default): 일반적인 문서 흐름에 따라 배치
  - top, right, bottom, left, z-index 속성이 아무런 영향도 주지 않는다
- relative: 일반적인 문서 흐름에 따라 배치
  - top, right, bottom, left의 값에 따라 오프셋을 적용한다
  - 오프셋은 다른 요소에 영향을 주지 않는다
  - 요소가 차지하는 공간은 static일 떄와 같다
- sticky: 일반적인 문서 흐름에 따라 배치하고, 가장 가까운 블록 레벨 조상을 기준으로 배치
  - static처럼 위치해 있다가 scroll이 해당 부분을 넘어가면 fixed처럼 위치한다
- fixed: 뷰포트의 초기 컨테이닝 블록를 기준으로 배치
  - 일반적인 문서 흐름에서 제거되어 페이지 레이아웃에 공간을 배정하지 않는다
- absolute: 조상 요소 중 positioning(static이 아닌 값) 된 가장 가까운 요소를 기준으로 배치
  - 일반적인 문서 흐름에서 제거되어 페이지 레이아웃에 공간을 배정하지 않는다
</details>


<details>
<summary>z-index란? (1)</summary>
<br>

- z-index: positioning된 요소, 그 자손과 flex items의 z축 순서를 지정한다
  - 정수 값을 사용한다
  - 숫자가 클 수록 앞으로 나온다
</details>


<details>
<summary>쌓임 맥락 이란? (1)</summary>
<br>

- 쌓임 맥락(stacking context)은 가상의 Z축을 사용한 HTML 요소의 3차원 개념화입니다. Z축은 사용자 기준이며, 사용자는 뷰포트 혹은 웹페이지를 바라보고 있을 것으로 가정합니다. 각각의 HTML 요소는 자신의 속성에 따른 우선순위를 사용해 3차원 공간을 차지합니다.
</details>


<details>
<summary>쌓임 맥락을 생성하는 요소에는 어떤 것들이 있나요? (16)</summary>
<br>

- 문서의 루트 요소 (`<html>`)
- `position`이 `absolute` 또는 `relative`이고, `z-index`가 `auto`가 아닌 요소
- `position`이 `fixed` 또는 `sticky`인 요소 (`sticky`는 모든 모바일 브라우저에서는 해당하지만 구형 데스크톱 브라우저에서는 해당하지 않음)
- 플렉스(`flexbox` (en-US)) 컨테이너의 자식 중 `z-index`가 `auto`가 아닌 요소.
- 그리드(`grid`) 컨테이너의 자식 중 `z-index`가 `auto`가 아닌 요소.
- `opacity`가 1보다 작은 요소
- `mix-blend-mode`가 `normal`이 아닌 요소
- 다음 속성 중 하나라도 `none`이 아닌 값을 가진 요소
	- `transform`
	- `filter`
	- `perspective` (en-US)
	- `clip-path`
	- `mask` / `mask-image` (en-US) / `mask-border` (en-US)
- `isolation`이 `isolate`인 요소
- `-webkit-overflow-scrolling`이 `touch`인 요소
- `will-change`의 값으로, 초깃값이 아닐 때 새로운 쌓임 맥락을 생성하는 속성을 지정한 요소
- `contain`이 `layout`, `paint`, 또는 둘 중 하나를 포함하는 값(`strict`, `content` 등)인 요소
</details>


<details>
<summary>쌓임 맥락은 어떤 특징이 있나요? (4)</summary>
<br>

- 하나의 쌓임 맥락은 부모 쌓임 맥락 안에서 통째로 하나의 단위로 간주됩니다.
- 쌓임 맥락이 다른 쌓임 맥락을 포함할 수 있고, 함께 계층 구조를 이룹니다.
- 쌓임 맥락은 형제 쌓임 맥락과 완전히 분리됩니다. 쌓임을 처리할 땐 자손 요소만 고려합니다.
- 각각의 쌓임 맥락은 독립적입니다. 어느 요소의 콘텐츠를 쌓은 후에는 그 요소를 통째 부모 쌓임 맥락 안에 배치합니다.
</details>

<details>
<summary>CSS position property value의 종류는? (5)</summary>
<br />

- `static`
	- position의 기본 값은 `static`이고, 이 경우 원래 있어야 할 위치인 HTML에 작성된 순서 그대로 브라우저 화면에 표시됩니다.
- `relative`
	- `relative` 는 요소의 원래 위치를 기준으로 상대적으로 배치합니다. 이때 요소의 원래 자리는 그대로 차지하고 있습니다. `top`, `bottom`, `left`, `right` 속성을 이용해서 요소의 원래 위치 기준 이동하도록 설정할 수 있습니다.
- `absolute`
	- `absolute` 는 가장 가까운 포지셔닝(`static` 이 아닌 position 속성 값)이 된 조상 요소를 기준으로 배치됩니다. 이때 글의 흐름에서 완전히 빠져서, 요소의 원래 자리는 차지하지 않습니다. 보통 상위 요소의 position 속성을 `relative` 로 지정하여 배치할 기준을 잡고 사용합니다.
- `fixed`
	- `fixed` 는 브라우저 전체 화면을 기준으로 고정된 배치입니다. `top`, `bottom`, `left`, `right` 속성은 브라우저의 상, 하, 좌, 우에서 해당 요소가 얼마나 떨어져 있는지를 결정합니다. 글의 흐름에서 완전히 빠져서, 요소의 원래 자리는 차지하지 않습니다. 내비게이션을 만들 때 많이 사용하는데, 요소의 원래 자리를 차지하지 않기 때문에 요소간 겹치지 않도록 마진을 넣어주기도 합니다.
- `sticky`
	- `sticky` 는 `static` 처럼 원래 위치에 배치해 있다가, 정해진 위치에 브라우저가 스크롤되면 그때부터 `fixed`처럼 고정되어 배치됩니다. 기본적으로는 `static` 처럼 배치하기 때문에 요소의 원래 자리를 차지합니다. `top`, `bottom`, `left`, `right` 설정이 필요하고, 가장 가까운 scroll되는 조상을 기준으로 배치 합니다.
</details>

<details>
  <summary>BEM이란? (5)</summary>
  <br />

  - BEM(Blcok Element Modifier)란 CSS 클래스 이름을 짓는 규칙입니다.
	- `Block` `<div>`같은 영역을 의미합니다.
	- `Element` `<button>`, `<input>`같은 요소를 의미합니다.
	- `Modifier` 요소의 변형을 표시하는 것을 의미합니다.
	- 이것들을 `.block__element--modifier` 형태로 씁니다.
</details>

<details>
<summary>BEM의 예시를 들어주세요. (2)</summary>
<br />

```html
<form class="signin-form">
	<label class="signin-form__label">
		Email
		<input type="text" class="signin-form__input">
	</label>
	<label class="signin-form__label">
		Password
		<input type="password" class="signin_form__input signin_form__input--pasword">
	</label>
	<button class="signin-form__button signin-form__button--submit">
		Sign In
	</button>
</form>

```

```css
.signin-form { /* 로그인 폼 */ }

.signin-form__input { /* 로그인 폼의 인풋 */ }

.signin-form__input.signin-form__input--password { /* 로그인 폼의 비밀번호 인풋 */ }

.signin-form__button { /* 로그인 폼의 버튼 */ }

.signin-form__button.signin-form__button--submit { /* 로그인 폼의 제출 버튼 */ }

```
</details>

<details>
<summary>Sass란? (3)</summary>
<br />

- CSS는 웹 표준이기 때문에 문법이 빠르게 바뀌지 않습니다. 그래서 개발자들이 사용하기 편한 여러가지 문법을 추가한 새로운 언어를 만들기 시작했는데, 그 중에 가장 많이 쓰이는 것이 바로 Sass입니다. 변수, 네스팅(Nesting) 문법, 믹스인(Mixin) 등등 다양한 기능을 제공합니다. 이 중에서 많은 사람들이 좋다고 생각한 문법(변수, 네스팅 등)은 웹 표준으로 흡수되기도 했습니다.
- Sass는 프리프로세서(Preprocessor) 스크립트 언어라고 하는데, 프리프로세서라는 프로그램을 통해서 Sass 코드를 CSS 코드로 변환하기 때문에 그렇습니다.
- Sass에는 기존 Sass와 SCSS 두 가지 문법이 있는데, 최근에는 CSS의 모든 문법 위에서 확장된 문법을 사용하는 SCSS를 많이 사용합니다.
</details>

<details>
<summary>네스팅(nesting)의 예시를 들어주세요 (1)</summary>
<br />
	
```css
nav {
  ul {
		margin: 0;
		padding: 0;
		list-style: none;
	}

	li { display: inline-block; }

	a {
		display: block;
		padding: 6px 12px;
		text-decoration: none;
	}
}

```
</details>

<details>
	<summary>믹스인(mixin)의 예시를 들어주세요 (1)</summary>
	<br />
	
Scss
```scss
@mixin theme($theme: DarkGray) {
  background: $theme;
  box-shadow: 0 0 1px rgba($theme, .25);
  color: #fff;
}

.info {
  @include theme;
}

.alert {
  @include theme($theme: DarkRed);
}

.success {
  @include theme($theme: DarkGreen);
}

```

CSS
```css
.info {
  background: DarkGray;
  box-shadow: 0 0 1px rgba(DarkGray, .25);
  color: #fff;
}

.alert {
  background: DarkRed;
  box-shadow: 0 0 1px rgba(DarkRed, .25);
  color: #fff;
}

.success {
  background: DarkGreen;
  box-shadow: 0 0 1px rgba(DarkGreen, .25);
  color: #fff;
}

```
</details>

<details>
<summary>CSS Modules란? (1)</summary>
<br />

- CSS Modules는 CSS 스타일을 모듈화하여 웹 개발 프로젝트에서 사용하는 기술입니다. 기존의 전역 스코프를 가진 CSS 규칙을 사용하는 방식과는 달리, CSS Modules는 각각의 모듈에 대해 스코프가 지정되어 스타일이 격리되고 충돌을 방지할 수 있습니다.
</details>

<details>
<summary>CSS Modules의 특징을 설명해주세요. (4)</summary>
<br />

- 모듈 스코핑(module scoping): 각각의 CSS 모듈은 고유한 스코프를 가지며, 스타일 규칙은 해당 모듈 내에서만 적용됩니다. 이렇게 하면 스타일 규칙이 전역으로 적용되어 생길 수 있는 충돌을 방지할 수 있습니다.
- 로컬 클래스 네임(local class names): CSS in Modules에서는 클래스 이름을 지정할 때 로컬 클래스 네임을 사용합니다. 이로써 클래스 이름이 충돌하지 않고 고유하게 유지됩니다. 일반적으로는 [파일이름]_[클래스이름]__randomString 형식으로 클래스 이름이 생성됩니다.
- 재사용 가능한 스타일(reusable styles): CSS in Modules에서는 스타일 규칙을 모듈로 정의하여 다른 모듈에서 재사용할 수 있습니다. 이를 통해 코드 중복을 줄이고 유지보수성을 향상시킬 수 있습니다.
- 스코프 범위 지정(scope control): CSS in Modules에서는 모듈 내에서만 스타일이 적용되는 것이 기본 동작입니다. 그러나 필요한 경우 전역 스타일을 사용할 수도 있습니다.
</details>

<details>
<summary>Tailwind CSS란? (1)</summary>
<br />

- Tailwind CSS는 Atomic CSS와 Utility-first 접근 방식을 적용한 현대적인 CSS 프레임워크입니다. Tailwind CSS는 개발자에게 유연하고 효율적인 스타일링을 제공하기 위해 다양한 사전 정의된 클래스를 제공합니다.
</details>

<details>
<summary>Atomic CSS와 Utility-first란? (2)</summary>
<br />

- Atomic CSS는 스타일을 작은, 독립적인 단위로 분해하여 클래스 단위로 정의하는 접근 방식입니다. 이러한 작은 단위를 `원자(Atom)`라고 부르며, 이러한 원자들을 조합하여 필요한 스타일을 생성합니다. 예를 들어, `padding-top: 10px`라는 스타일을 정의하는 대신 `pt-10`이라는 클래스를 사용하는 식으로 스타일을 적용합니다. Atomic CSS는 스타일 규칙을 재사용 가능한 단위로 만들어 코드의 효율성과 유지보수성을 높이는 데 중점을 둡니다.
- Utility-first는 Atomic CSS의 변형으로, 스타일을 구성하는 작은 원자들을 재사용 가능한 유틸리티 클래스로 구성하는 방식입니다. 이 방식에서는 스타일 규칙을 간결한 클래스 이름으로 표현하고 이러한 클래스를 HTML 요소에 직접 적용하여 스타일을 적용합니다. 예를 들어, "text-center"이라는 클래스를 사용하여 텍스트를 가운데 정렬하는 스타일을 적용할 수 있습니다. Utility-first는 반복되는 스타일을 간결하게 표현하고 재사용 가능한 클래스로 관리함으로써 개발자에게 빠르고 효율적인 스타일링을 제공합니다.
</details>

<details>
<summary>CSS 기술들의 장단점을 설명해주세요. (6)</summary>
<br />

- 전통적인 CSS
	- CSS 클래스 이름을 짓는 것이 번거롭습니다.
	- CSS 클래스 이름이 충돌할 가능성이 있습니다.
	- 코드의 규모가 커지면 관리가 어렵습니다.
	- 작성한 코드를 브라우저가 그대로 실행하기 때문에 추가적인 연산이 발생하지 않는다는 장점이 있습니다.
- BEM 방법론
	- CSS 클래스의 이름을 짓는 고민을 덜 수 있습니다.
	- 여전히 규모가 큰 코드를 관리하기는 어렵습니다.
- Sass와 같은 CSS Preprocessor
	- 여전히 CSS 클래스 이름이 충돌할 가능성이 있습니다.
	- 파일을 분리하고 불러 올 수 있기 때문에 규모가 큰 코드를 관리하기 좋습니다.
	- 반복되는 CSS 코드를 줄여주는 다양한 문법이 있어서 작업 효율이 좋습니다.
- CSS Modules
	- 컴포넌트 단위로 나누어서 스타일링할 수 있어서 CSS 클래스 이름이 충돌하지 않습니다.
	- 필요하다면 Sass로 CSS Modules를 사용할 수 있습니다. (create-react-app 에서는 자체적으로 [Sass와 CSS modules를 함께 사용하도록](https://create-react-app.dev/docs/adding-a-css-modules-stylesheet/) 해 줍니다.)
- CSS-in-JS
	- 컴포넌트 단위로 나누어서 스타일링할 수 있어서 CSS 클래스 이름이 충돌하지 않습니다.
	- 클래스네임을 짓지 않아도 됩니다.
	- 자바스크립트와 JSX로 된 컴포넌트 코드와 스타일링 코드가 한 파일에 있어서 관리하기 좋습니다.
	- 하지만 자바스크립트를 실행해서 CSS를 만들기 때문에 CSS나 Sass에 비해서 추가적인 연산이 필요합니다. 그리고 렌더링 속도도 훨씬 느려진다는 단점이 있습니다.
- Tailwind CSS와 같은 Utility-first(Atomic CSS)
	- CSS 클래스를 나누는 기준을 컴포넌트나 디자인이 아닌 작은 단위의 CSS 속성으로 두기 때문에, CSS 클래스 이름 충돌에 대한 걱정이 없습니다.
	- 보편적으로 사용하는 CSS 클래스를 여러 컴포넌트에서 공유하기 때문에, 규모가 큰 프로젝트더라도 CSS 코드의 양이 굉장히 적다는 장점이 있습니다.
	- CSS-in-JS와 마찬가지로 JSX로 된 컴포넌트 코드와 스타일링 코드가 한 파일에 있어서 관리하기 좋습니다.
	- 복잡한 디자인을 적용할 때에는 CSS 클래스가 한없이 길어져서 가독성이 떨어지고 관리하기 어렵다는 단점이 있습니다.
	- 그래서 Tailwind CSS 같은 경우 별도의 문법([@apply](https://tailwindcss.com/docs/reusing-styles#extracting-classes-with-apply))으로 추상화를 지원하기도 합니다.

```tsx
<a href="..." className="rounded-lg px-3 py-2 text-slate-700 font-medium hover:bg-slate-100 hover:text-slate-900">...</a>

```
</details>
