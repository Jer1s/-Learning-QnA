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
<summary>()</summary>
<br>

- 
</details>

<details>
<summary>()</summary>
<br>

- 
</details>

<details>
<summary>()</summary>
<br>

- 
</details>

<details>
<summary>()</summary>
<br>

- 
</details>

<details>
<summary>()</summary>
<br>

- 
</details>

<details>
<summary>()</summary>
<br>

- 
</details>

<details>
<summary>()</summary>
<br>

- 
</details>

<details>
<summary>()</summary>
<br>

- 
</details>

<details>
<summary>()</summary>
<br>

- 
</details>

<details>
<summary>()</summary>
<br>

- 
</details>

<details>
<summary>()</summary>
<br>

- 
</details>





