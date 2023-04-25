<details>
<summary>리액트(React)의 탄생 배경과 역사에 대해 설명해주세요. (5)</summary>
<br>

- React의 탄생 배경은 Facebook이 직면한 문제에서 시작됩니다. Facebook은 커다란 규모의 복잡한 웹 애플리케이션을 유지보수하고 개발하는데 어려움을 겪고 있었습니다. 그러한 문제 중에서도 가장 큰 문제 중 하나는 자주 일어나는 UI 변경으로 인한 성능 저하와 유지보수성의 어려움이었습니다.
- 이러한 문제를 해결하기 위해 Facebook에서는 더 나은 방법을 찾기 위해 여러 가지 실험을 진행했습니다. 그 중에서도 React는 Jordan Walke라는 개발자가 2011년에 시작한 프로젝트였습니다. React는 JavaScript 라이브러리로, 가상 DOM(Virtual DOM) 개념을 도입하여 성능을 개선하고, 컴포넌트라는 개념을 도입하여 UI 코드를 모듈화하고 재사용성을 높였습니다.
- React는 초기 버전에서는 Facebook에서 사용하기 위해 개발되었으며, 2013년에 5월에 오픈 소스로 최초로 공개되었습니다. 그 후 React는 계속해서 발전하면서 다양한 기능과 개선 사항이 추가되었고, 2015년 Facebook에서 React Native라는 모바일 애플리케이션을 위한 새로운 크로스플랫폼 프레임워크도 출시했습니다.
- React의 등장으로 인해 UI 코드의 개발과 유지보수가 쉬워졌고, 성능 또한 향상되어 대규모 웹 애플리케이션을 개발할 수 있게 되었습니다. 이로 인해 React는 현재까지도 많은 개발자들에게 사랑받고 있으며, 대규모 웹 애플리케이션의 개발에서는 필수적인 기술 중 하나입니다.
- React는 지속적으로 개발이 이루어지고 있으며, 현재는 React 18 버전이 개발 중에 있습니다. React의 생태계는 매우 다양하며, React를 기반으로 한 다양한 라이브러리와 프레임워크가 존재합니다.
</details>

<details>
<summary>리액트 프로젝트를 만드는 방법에 대해 설명해주세요. (2)</summary>
<br>

1. Create React App(CRA) 사용하기
    - Create React App(CRA)은 리액트 앱을 빠르게 만들기 위한 공식 도구입니다.
    - CRA를 사용하면, 초기 세팅을 자동으로 생성하고, 빠르게 리액트 앱을 만들 수 있습니다.
    - 아래는 CRA를 사용하여 리액트 앱을 만드는 방법입니다.

      1. Node.js를 설치합니다.

      2. 터미널에서 다음 명령어를 실행합니다.

        ```console
        npx create-react-app my-app
        ```

      3. 생성된 앱 폴더로 이동하여 개발모드를 실행합니다.

        ```kotlin
        cd my-app
        npm start
        ```

2. 수동으로 세팅하기
    - 아래는 수동으로 리액트 앱을 만드는 방법입니다.

      1. Node.js를 설치합니다.

      2. 리액트 프로젝트에 필요한 패키지를 설치합니다.
        ```kotlin
        npm init -y
        npm install react react-dom
        npm install -D webpack webpack-cli webpack-dev-server html-webpack-plugin babel-loader @babel/core @babel/preset-env @babel/preset-react
        ```

      3. 프로젝트 디렉토리에 다음과 같은 파일들을 생성합니다.

        ```bash
        /public/index.html
        /src/index.js
        /webpack.config.js
        /.babelrc
        ```

      4. 생성한 파일들을 수정하여 리액트 앱을 만듭니다.

        ```jsx
        // index.html
        <!DOCTYPE html>
        <html>
        <head>
          <meta charset="UTF-8">
          <title>My React App</title>
        </head>
        <body>
          <div id="root"></div>
          <script src="dist/bundle.js"></script>
        </body>
        </html>

        // index.js
        import React from 'react';
        import ReactDOM from 'react-dom';
        import App from './App';

        ReactDOM.render(<App />, document.getElementById('root'));
        ```

</details>

<details>
<summary>React Developer Tools란? (3)</summary>
<br>

- React Developer Tools는 React 애플리케이션의 디버깅 및 프로파일링을 도와주는 크롬 확장 프로그램입니다.
- React Developer Tools를 사용하면 React 구성 요소 트리와 해당 구성 요소의 속성 및 상태를 시각적으로 볼 수 있습니다.
- React Developer Tools를 사용하면 React 애플리케이션의 성능을 프로파일링하여 느린 부분을 파악하고 최적화할 수 있습니다.
</details>

<details>
<summary>React에서 index.html이 하는 일에 대해 설명해주세요. (4)</summary>
<br>

- React 애플리케이션이 실행될 때 웹 브라우저에서 가장 먼저 실행되는 파일입니다.
- `public` 디렉토리에 있어야 합니다.
- React 애플리케이션이 렌더링될 때 사용되는 루트 요소(root element)를 포함합니다.
- React 애플리케이션에서는 일반적으로 index.html 파일이 동적으로 생성된 JavaScript 파일을 로드하고 실행하기 위해 사용됩니다.
</details>

<details>
<summary>React에서 index.js가 하는 일에 대해 설명해주세요. (6)</summary>
<br>

- React 애플리케이션의 시작점(Entry point)으로, 컴포넌트들을 불러오고 렌더링하는 역할을 담당합니다.
- 일반적으로 src 디렉토리에 위치합니다.
- React 17부터는 React를 import하지 않고도 JSX 문법을 사용할 수 있도록 변경되었습니다.
- `createRoot()` 이 메소드는 React 18에서 추가된 새로운 API 중 하나이며, ReactDOM 패키지의 일부입니다. 이 메소드는 React 애플리케이션의 루트 엘리먼트를 선택하고, 이를 관리할 Root 객체를 리턴합니다.
- `render()` Root 객체의 렌더 메소드를 호출하여 JSX를 사용하여 작성된 엘리먼트를 렌더링합니다.
- 이전 버전의 React에서는 `createRoot()` 메소드 대신에 `ReactDOM.render()` 메소드를 사용하여 렌더링을 처리했었습니다.
</details>

<details>
<summary>JSX란? (4)</summary>
<br>

- JSX는 JavaScript Syntax Extension, JavaScript XML의 약자로, JavaScript를 확장한 문법입니다.
- JSX는 JavaScript와 유사한 XML 형태의 문법을 사용하여 UI 컴포넌트를 정의하고 렌더링할 수 있습니다.
- React에서 UI 컴포넌트를 작성할 때 사용되는 기술입니다.
- JSX를 사용하면 HTML과 비슷한 구문으로 React 컴포넌트를 작성할 수 있으며, 가독성이 좋고 개발 생산성을 향상시킬 수 있습니다.
</details>

<details>
<summary>JSX에서 주의해야할 문법은? (5)</summary>
<br>

- `Self-closing tag`
  - JSX에서는 일반적인 HTML과 달리, self-closing 태그를 사용할 때 '/'를 생략할 수 없습니다.
- `camelCase attribute name`
  - JSX에서는 속성명을 camelCase 형태로 작성해야 합니다.
  - 예시
    - `onClick`
    - `onBlur`
    - `onFocus`
    - `onMouseDown`
    - `onMouseOver`
    - `tabIndex`
  - 예외적으로 HTML에서 비표준 속성을 다룰 때 활용하는 `data-*` 속성은 camelCase가 아니라 기존의 HTML 문법 그대로 작성해야 합니다.
- `htmlFor`
  - JSX에서는 for 속성이 예약어이기 때문에 for 대신 htmlFor 속성을 사용해야 합니다.
- `className`
  - JSX에서는 class 속성이 예약어이기 때문에 class 대신 className 속성을 사용해야 합니다.
- `style attribute`
  - HTML에서는 스타일 속성을 문자열 형태로 지정할 수 있지만, JSX에서는 JavaScript 객체 형태로 스타일을 정의해야 합니다.
  - 예를 들어, `<div style="color: red;"></div>` 대신 `<div style={{ color: "red" }}></div>`와 같이 작성해야 합니다.
</details>

<details>
<summary>Fragment란? (4)</summary>
<br>
    
- JSX에서 여러 요소를 렌더링하려면, 이를 하나의 컨테이너 요소로 감싸주어야 합니다.
- 이때, 불필요한 div 태그를 사용하지 않기 위해 Fragment를 사용할 수 있습니다.
- Fragment는 빈 태그로, `<>` `</>`와 같이 작성합니다.
- `react`에서 `{ Fragment }`를 import해서 `<Fragment>` `</Fragment>`와 같이 작성할 수도 있습니다.
</details>

<details>
<summary>JSX에서 자바스크립트 코드를 삽입하는 방법에 대해 설명해주세요. (3)</summary>
<br>

- JSX에서 자바스크립트 코드를 삽입할 때는 중괄호({})를 사용합니다.
- 중괄호 안에는 유효한 자바스크립트 표현식을 작성해야 합니다.
- 중괄호 안에는 if문, for문 또는 함수 선언과 같은 자바스크립트의 문장은 사용할 수 없습니다.
</details>

<details>
<summary>리액트 엘리먼트란? (5)</summary>
<br>

- 리액트 엘리먼트(React element)는 React에서 UI를 표현하는 가장 작은 단위입니다.
- 리액트 엘리먼트는 일반적으로 JSX 문법을 사용하여 작성됩니다.
- 리액트 엘리먼트는 JavaScript 객체입니다.
- 각 엘리먼트는 해당 엘리먼트의 타입(type), 속성(props), 자식 엘리먼트(children)를 포함합니다.
- 예시
    ```jsx
    const element = <h1>Hello, world!</h1>;
    ```
</details>

<details>
<summary>리액트 컴포넌트란? (5)</summary>
<br>

- 리액트 컴포넌트(React component)는 UI를 작은 단위로 나누어서 재사용 가능한 코드로 만드는 방법입니다.
- 리액트 컴포넌트는 JSX 문법으로 만든 리액트 엘리먼트를 리턴해야 합니다.
- 리액트 컴포넌트는 UI의 각 부분을 캡슐화하고, 각각의 부분을 독립적으로 개발, 테스트, 유지보수할 수 있도록 도와줍니다.
- 리액트 컴포넌트의 이름의 첫 글자는 대문자로 작성해야 합니다.
- 리액트 컴포넌트는 함수 컴포넌트와 클래스 컴포넌트로 구현할 수 있습니다.
</details>

<details>
<summary>함수 컴포넌트란? (3)</summary>
<br>

- 함수 컴포넌트(function component)는 입력(props)을 받아서 UI를 리턴하는 함수로 정의되는 리액트 컴포넌트입니다.
- 함수 컴포넌트는 HTML의 커스텀 태그처럼 활용할 수 있습니다.
- 예시
```jsx
function my_func(props) {
  return reactComponent;
}
```
</details>

<details>
<summary>클래스 컴포넌트란? (7)</summary>
<br>

- 클래스 컴포넌트(class component)는 `React.Component` 클래스를 상속하여 정의되는 리액트 컴포넌트입니다.
- 클래스 컴포넌트는 상태(state)나 라이프사이클(lifecycle) 메소드를 사용할 수 있으며, 다양한 메소드를 구현하여 컴포넌트의 동작을 제어할 수 있습니다.
- 클래스 컴포넌트는 `render()` 메소드를 반드시 구현해야 합니다.
- `render()` 메소드는 컴포넌트의 UI를 반환하는 함수입니다.
- 클래스 컴포넌트에서 상태(state)를 사용하려면, `constructor()` 메소드에서 this.state 객체를 초기화하고, `setState()` 메소드를 사용하여 상태를 업데이트해야 합니다.
- `setState()` 메소드를 호출하면 React는 상태를 변경하고, `render()` 메소드를 호출하여 UI를 업데이트합니다.
- 예시
    ```jsx
    class Counter extends React.Component {
      constructor(props) {
        super(props);
        this.state = { count: 0 };
      }

      handleClick() {
        this.setState({ count: this.state.count + 1 });
      }

      render() {
        return (
          <div>
            <div>Count: {this.state.count}</div>
            <button onClick={() => this.handleClick()}>Click me</button>
          </div>
        );
      }
    }
    ```
</details>

<details>
<summary>Props란? (5)</summary>
<br>

- 리액트에서 Props(Properties)는 부모 컴포넌트로부터 자식 컴포넌트로 전달되는 데이터를 말합니다.
- Props는 읽기 전용(read-only)이며, 자식 컴포넌트에서 변경할 수 없습니다.
- Props는 객체 형태로 전달되며, 자식 컴포넌트에서는 Props를 파라미터로 받아와 사용할 수 있습니다. 이 때 `destructuring`을 활용할 수 있습니다.
- 클래스 컴포넌트에서는 this.props를 사용하여 Props를 받아올 수 있습니다.
- 예시 (`destructuring`, `default parameter` 사용)
    ```jsx
    // src/Dice.js
    import ...

    const DICE_IMAGES = {
      blue: [diceBlue01, diceBlue02, diceBlue03, diceBlue04, diceBlue05, diceBlue06],
      red: [diceRed01, diceRed02, diceRed03, diceRed04, diceRed05, diceRed06],
    };

    function Dice({ color = 'blue', num = 1 }) {
      const src = DICE_IMAGES[color][num - 1];
      const alt = `${color} ${num}`;
      return <img src={src} alt={alt} />;
    }

    export default Dice;
    ```
</details>

<details>
<summary>children이란? (2)</summary>
<br>

- 리액트 컴포넌트 태그 사이에 내용을 보여주는 props 속성입니다.
- 자식 컴포넌트에서 `props.children`으로 접근할 수 있습니다.
</details>

<details>
<summary>State란? (2)</summary>
<br>

- React 컴포넌트에서 관리되는 객체로, 클래스 컴포넌트의 상태를 저장하고 변경할 수 있는 데이터입니다.
- React state는 setState() 메소드를 사용하여 업데이트됩니다. setState() 메소드를 호출하면 react는 컴포넌트를 다시 렌더링하고 변경된 state를 적용합니다.
</details>

<details>
<summary>useState()란? (3)</summary>
<br>

- `useState()`는 React Hooks API에서 제공하는 함수 중 하나로, 함수형 컴포넌트에서도 state를 사용할 수 있게 해줍니다.
- `useState()` 함수는 배열을 반환하며, 첫 번째 요소는 현재 상태 값이고, 두 번째 요소는 해당 상태 값을 업데이트하고 컴포넌트를 다시 렌더링하는 setter 함수입니다.
- `useState()`의 파라미터는 현재 상태 값의 초기값을 저장합니다.
</details>

<details>
<summary>참조형 state란? (3)</summary>
<br>

- 참조형 state는 객체, 배열, 클래스 등의 참조형 타입을 저장한 state입니다.
- 참조형 state의 setter 함수에 내부 값만 변경한 state를 전달할 경우, 참조하는 주소 값이 변경되지는 않기 때문에 react가 컴포넌트를 다시 렌더링하지는 않습니다.
- 간단하게 `...object` spread 문법으로 복사한 참조형 state를 setter 함수에 전달해서 해결할 수 있다.
  - spread 연산자를 사용한 객체 복사는 깊은 복사가 아니기 때문에, 객체 안의 객체가 있을 경우에 같은 문제가 발생할 수 있다.
  - 이 때에는 `Lodash`나 `Immer`같은 라이브러리를 사용하거나, `JSON.stringify()`와 `JSON.parse()` 함수를 이용하여 객체를 문자열로 변환한 후 다시 객체로 변환하는 방법, 또는 재귀 함수를 이용한 깊은 복사를 하여 해결할 수 있다.
</details>

<details>
<summary>컴포넌트 사용의 이점을 설명해주세요. (3)</summary>
<br>

- 반복적인 개발이 줄어듭니다.
- 오류를 고치기 쉽습니다.
- 일을 쉽게 나눌 수 있습니다.
</details>

<details>
<summary>State lifting이란? (2)</summary>
<br>

- React에서 `state lifting`은 부모 컴포넌트로부터 자식 컴포넌트로 상태를 전달하고 업데이트하는 기술입니다.
- 부모 컴포넌트가 자식 컴포넌트의 상태를 업데이트하면, 이를 사용하는 모든 하위 컴포넌트가 자동으로 업데이트되므로 코드의 일관성과 유지보수성을 높일 수 있습니다.
</details>

<details>
<summary>렌더링(Rendering)이란? (3)</summary>
<br>

- 컴퓨터 그래픽스에서 모델링된 데이터를 시각적으로 표현하는 과정입니다.
- 웹 개발에서는 브라우저에 HTML, CSS, JavaScript 등의 웹 문서를 표시하기 위한 과정을 말합니다.
- 웹 페이지가 브라우저에 표시되기 위해서는 HTML 문서가 브라우저에서 파싱되고, CSS 스타일이 적용되며, JavaScript 코드가 실행되어야 합니다. 이러한 과정을 거쳐 브라우저가 화면에 웹 페이지를 렌더링합니다.
</details>

<details>
<summary>서버 사이드 렌더링(Server-Side Rendering, SSR)이란? (6)</summary>
<br>

- 웹 서버에서 HTML 코드를 생성하여 클라이언트에게 전송하는 방식입니다.
- 서버 사이드 렌더링을 구현하려면 서버에서 웹 페이지를 동적으로 생성해야 합니다.
- 서버 사이드 렌더링은 초기 로딩 속도를 빠르게 하고, 검색 엔진 최적화(SEO)에 유리합니다.
- 서버 사이드 렌더링은 초기 로딩 속도를 빠르게 하기 위해 SPA(Single-Page Application)에서도 사용될 수 있습니다.
- SPA에서는 일반적으로 CSR 방식을 사용하지만, 초기 로딩 속도를 빠르게 하기 위해 SSR을 사용하는 방법도 있습니다.
- React 프레임워크에서는 서버 측에서 `ReactDOMServer.renderToString()` 메소드를 사용하여 리액트 컴포넌트를 렌더링할 수 있습니다. 이를 통해 서버에서 생성된 HTML 코드를 클라이언트에 전달하면 클라이언트는 이를 그대로 사용할 수 있습니다.
</details>

<details>
<summary>클라이언트 사이드 렌더링(Client-Side Rendering, CSR)이란? (5)</summary>
<br>

- 웹 브라우저에서 JavaScript를 사용하여 HTML 코드를 동적으로 생성하는 방식입니다.
- React, Angular, Vue.js 등의 프론트엔드 프레임워크는 CSR 방식을 사용합니다.
- CSR 방식은 SPA(Single-Page Application)에서 많이 사용됩니다.
- SPA에서는 모든 컨텐츠가 하나의 페이지에서 로드되므로, 초기 로딩 속도가 느리더라도 한 번 로딩되면 나머지 페이지 전환 시간이 매우 빠릅니다.
- CSR 방식에서는 서버에서 단순히 JSON 데이터만 전송하므로, 서버 측에서도 부하를 줄일 수 있습니다.
</details>

<details>
<summary>리액트의 렌더링 과정에 대해 설명해주세요. (4)</summary>
<br>

1. 컴포넌트가 렌더링될 때, React는 해당 컴포넌트의 가상 DOM을 생성합니다. 이 가상 DOM은 React 요소(React element)와 컴포넌트의 상태(state) 및 속성(props) 정보를 포함합니다.
2. 생성된 가상 DOM은 이전에 렌더링된 가상 DOM과 비교됩니다. 이를 위해 React는 이전 가상 DOM과 현재 가상 DOM을 비교하여 변경된 부분을 파악합니다. 이 과정을 "재조정(reconciliation)"이라고 합니다.
3. 변경된 부분을 파악한 후, React는 이전 가상 DOM과 현재 가상 DOM 간의 차이를 최소화하기 위해 최소한의 업데이트만 수행합니다. 이를 "미세조정(optimization)"이라고 합니다.
4. 변경된 부분만 실제 DOM에 반영됩니다.
</details>

<details>
<summary>리액트의 렌더링 방식의 장점에 대해 설명해주세요. (2)</summary>
<br>

- 리액트는 필요한 최소한의 업데이트만 수행하면서도 빠르고 효율적인 렌더링을 구현할 수 있습니다.
- 리액트는 상태(state)나 속성(props)이 변경될 때마다 자동으로 렌더링을 수행하므로, 개발자가 직접 DOM 조작을 수행할 필요가 없습니다. 이는 코드의 가독성과 유지보수성을 높여줍니다.
</details>

<details>
<summary>가상 DOM(Virtual DOM)이란? (2)</summary>
<br>

- Virtual DOM은 React에서 사용되는 가상의 DOM 객체 모델입니다.
- 실제 DOM은 브라우저에서 웹 페이지를 표시하기 위해 생성되는 객체 모델로, HTML 문서의 구조와 내용을 나타냅니다. 이에 반해, Virtual DOM은 React의 컴포넌트 구조와 상태를 나타내는 객체 모델로, 브라우저 상에 존재하지 않습니다.
</details>

<details>
<summary>가상 DOM의 특징에 대해 설명해주세요. (3)</summary>
<br>

- 성능 개선: Virtual DOM은 실제 DOM과는 별도로 존재하므로, 변경이 발생했을 때 전체 DOM을 다시 그리는 것이 아니라, 변경된 부분만 업데이트하여 성능을 개선할 수 있습니다.
- 브라우저 독립성: Virtual DOM은 브라우저에 종속되지 않기 때문에, 서버에서도 렌더링이 가능합니다. 이는 검색 엔진 최적화(SEO)에 유리하며, 초기 로딩 속도를 높일 수 있습니다.
- 개발 생산성 향상: Virtual DOM은 컴포넌트 단위로 작성할 수 있으므로, 코드의 가독성과 유지보수성을 높여줍니다.
</details>

<details>
<summary>React에서 인라인 스타일을 적용하는 방법에 대해 설명해주세요. (5)</summary>
<br>

- `<button style={style} />` 형식으로 인라인 스타일을 적용할 수 있습니다.
- 중괄호 안에 들어갈 `style`은 객체 형태로 스타일 정보를 전달해야 합니다.
- `style` 안의 property name은 camelCase로 작성해야하고, property value는 문자열로 작성해야 합니다.
- 객체 내에서 spread 문법을 활용할 수도 있습니다.
- 예시
    ```jsx
    const baseButtonStyle = {
      padding: '14px 27px',
      outline: 'none',
      cursor: 'pointer',
      borderRadius: '9999px',
      fontSize: '17px',
    };

    const blueButtonStyle = {
      ...baseButtonStyle,
      border: 'solid 1px #7090ff',
      color: '#7090ff',
      backgroundColor: 'rgba(0, 89, 255, 0.2)',
    };

    const redButtonStyle = {
      ...baseButtonStyle,
      border: 'solid 1px #ff4664',
      color: '#ff4664',
      backgroundColor: 'rgba(255, 78, 78, 0.2)',
    };
    ```
</details>

<details>
<summary>빌드(build)란? (3)</summary>
<br>

- 빌드는 소스 코드를 처리하여 애플리케이션을 구동하기 위한 최적화된 정적 파일을 생성하는 과정을 말합니다.
- React 애플리케이션을 배포할 때는, 빌드된 파일들을 웹 서버에 호스팅하여 사용자들이 접근할 수 있도록 합니다.
- 빌드된 파일은 개발 환경에서 실행하는 경우에 비해 더 빠르게 로딩되며, 애플리케이션의 성능과 안정성을 향상시킬 수 있습니다.
</details>

<details>
<summary>빌드 과정에 대해 설명해주세요. (3)</summary>
<br>

1. 코드 번들링(code bundling): 애플리케이션에 사용된 모든 JavaScript, CSS, 이미지 등의 파일들을 번들(bundle)로 묶어줍니다. 번들링을 하면 파일 요청 수를 줄여서 초기 로딩 속도를 개선할 수 있습니다.
2. 최적화: 코드를 최적화하여 파일 크기를 줄이고, 불필요한 코드를 제거합니다. 이를 통해 애플리케이션의 로딩 속도를 개선할 수 있습니다.
3. 소스 맵 생성: 소스 맵(Source Map)은 빌드된 파일과 원본 소스 코드 간의 대응 관계를 정의한 맵 파일입니다. 디버깅 시 원본 소스 코드에서 오류를 확인할 수 있도록 도와줍니다.
</details>

<details>
<summary>클라우드 컴퓨팅(Cloud computing)이란? (3)</summary>
<br>

- 인터넷을 통해 컴퓨팅 서비스를 제공하는 기술입니다.
- IaaS(Infrastructure as a Service), PaaS(Platform as a Service), SaaS(Software as a Service) 등의 다양한 서비스 모델을 제공합니다.
- Amazon Web Services(AWS), Microsoft Azure, Google Cloud Platform(GCP), Heroku, IBM Cloud, Oracle Cloud, Alibaba Cloud, Naver Cloud Platform 등의 클라우드 서비스 제공업체가 있습니다.
</details>

<details>
<summary>트랜스파일링(Transpiling)이란? (4)</summary>
<br>

- 트랜스파일링(Transpiling)은 하나의 프로그래밍 언어로 작성된 코드를 다른 프로그래밍 언어로 변환하는 것을 말합니다.
- 트랜스파일링은 주로 최신 문법을 지원하지 않는 브라우저에서도 실행 가능한 코드로 변환하기 위해 사용됩니다.
- 트랜스파일링을 위해서는 대표적으로 Babel이라는 도구를 사용합니다.
  - Babel은 ES6+ 자바스크립트 코드를 ES5 이하 버전의 자바스크립트 코드로 변환하는 기능뿐만 아니라, 다양한 플러그인을 제공하여 코드의 특정 기능을 지원하지 않는 브라우저에서도 동작할 수 있는 코드로 변환하는 작업을 수행합니다.
</details>

<details>
<summary>번들링(Bundling)이란? (4)</summary>
<br>

- 번들링(Bundling)은 여러 개의 파일들을 하나의 파일로 묶는 작업을 말합니다.
- 번들링을 하면 파일 요청 수와 파일 크기가 줄어들어 웹 페이지 로딩 속도가 빨라지는 장점이 있습니다.
- 번들링을 통해 개발자는 여러 개의 파일로 작업하는 대신 하나의 번들 파일로 작업할 수 있으며, 번들링된 파일을 웹 페이지에 삽입하여 사용할 수 있습니다.
- 번들링 도구로는 webpack, Parcel, Rollup 등이 있으며, 이들 도구는 여러 모듈들을 하나의 번들 파일로 묶어주는 역할을 합니다.
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>

<details>
<summary> (3)</summary>
<br>

- 
</details>
