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
<summary>z-index란? (2)</summary>
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
	
