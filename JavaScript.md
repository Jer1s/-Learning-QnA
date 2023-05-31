<details>
<summary>JavaScript란? (8)</summary>
<br>

- HTML, CSS와 함께 World Widw Web의 중요 기술 중 하나인 JIT 컴파일 프로그래밍 언어
- JavaScript는 웹 페이지에서 동적인 기능을 추가하고, 사용자와 상호작용하는 등 다양한 기능을 수행할 수 있습니다.
- JavaScript는 객체 지향 언어로, 변수, 함수, 클래스, 객체 등의 기본적인 프로그래밍 요소를 갖추고 있습니다.
- 브라우저에서 제공되는 Document Object Model (DOM)과 Browser Object Model (BOM)을 사용하여 웹 페이지의 요소에 접근하고 조작할 수 있습니다.
- JavaScript는 브라우저에서 실행되기 때문에, 어떠한 특별한 설치 없이 모든 브라우저에서 실행될 수 있습니다.
- Node.js라는 서버 측 JavaScript 실행 환경을 사용하여 서버 측 개발도 가능합니다.
- 2015년에 ES6 (ES2015) JavaScript 버전 업데이트를 기점으로 사용량이 크게 늘었습니다.
- Mobile application, pc application, VR, AR, block chain 등 다양한 분야에 활용되는 범용되는 기술로 발전했습니다.
</details>

<details>
<summary>JIT 컴파일 프로그래밍 언어란? (5)</summary>
<br>

- `JIT compiler` Just-In-Time의 준말으로, 런타임 시점에 코드를 컴파일하는 방식을 말합니다.
- `JIT compile programing language` 
  - JIT 컴파일러를 사용한 언어
  - 이를 통해 실행 속도를 향상시키고, 메모리 사용량을 줄일 수 있습니다.
  - 대표적인 JIT 컴파일 프로그래밍 언어로는 Java, C#, JavaScript(V8 엔진), Python(PyPy) 등이 있습니다.
</details>

<details>
<summary>JavaScript에서 Semi colon의 의미를 설명해주세요. (3)</summary>
<br>

- 한 문장 맨 끝에 세미콜론(;)을 붙여 문장을 구분합니다.
- Javascript는 코드를 해석하는 과정에서 상황에 따라 자동으로 세미콜론을 추가해주는 규칙이 있습니다.
- 필요한 경우에만 사용하는 사람도 있고 반드시 사용하는 사람이 있습니다.
</details>

<details>
<summary>JavaScript에서 comment를 다는 법을 설명해주세요. (1)</summary>
<br>

- `//` 뒤, `/* */` 사이의 내용은 실행되지 않습니다.
</details>

<details>
<summary>변수 선언자(variable declarator)은 어떤 것이 있나요? (3)</summary>
<br>

- var
  - function scope를 또는 global scope를 갖습니다.
  - var 키워드 변수 선언은 코드가 실행되기 전에 처리하기 때문에 hoisting이 일어납니다.
- let(ES6)
  - block scope 또는 global scope를 갖습니다.
- const(ES6)
  - block scope 또는 global scope를 갖는다
  - 해당 scope 내에서 할당된 값을 변경하거나 재선언 할 수 없습니다.
  - reference type을 할당할 경우 주소값이 복사되어 내부 요소의 값을 변경할 수 있습니다.
</details>

<details>
<summary>Variable naming rule 중 필수 규칙을 설명해주세요. (4)</summary>
<br>

- JavaScript 식별자는 '문자(a-z,A-Z)', '밑줄(\_)' 혹은 '달러 기호($)'로 시작해야 합니다.
- 두 번째 글자부터는 '숫자(0-9)'도 쓸 수 있습니다.
- 대문자와 소문자를 구분합니다.
- 예약어(Reserved word)는 사용할 수 없습니다. (Ex. if, for, let, this, ...)
</details>

<details>
<summary>Variable naming rule 중 선택 규칙을 설명해주세요. (3)</summary>
<br>

- 추상화와 구체화가 적당한 이름이 좋습니다.
- 이름에 의미를 담는 것이 좋습니다.
- 'camelCase'로 쓰는 것이 좋습니다.
</details>

<details>
<summary>function 선언, 호출 방법을 설명해주세요. (2)</summary>
<br>

- `function my_func(parameters) {statements}` 형태로 선언합니다.
- `my_func(arguments);` 형태로 호출합니다.
</details>

<details>
<summary>Parameter란? (4)</summary>
<br>

- 함수를 호출할 때 괄호 안에 parameter를 넣어 전달하면 함수 내부에서 사용할 수 있습니다.
- 전달되지 않은 parameter는 undefined 값으로 설정됩니다.
- Default parameter로 전달되지 않았을 때의 기본값을 설정할 수 있습니다.
- Default parameter는 뒷쪽에 쓰는 것이 좋습니다.
</details>

<details>
<summary>Return이란? (1)</summary>
<br>

- 함수가 실행된 자리에 값을 전달할 수 있게 해줍니다.
</details>

<details>
<summary>JavaScript에서 ==, ===의 차이점은? (3)</summary>
<br>

- `==` 는 느슨한 같음(loose equality)으로 두 값이 같은지 비교합니다. 이때, 두 값을 공통 형(type)으로 암묵적으로 변환합니다. 암묵적 변환은 서로 다른 타입이면 `Number` 타입으로 변환하고 최종 같음 비교는 `===` 처럼 수행됩니다.
  1. 두 값의 타입이 같으면 그대로 비교합니다.
  2. 두 값의 타입이 다르면 다음과 같은 규칙으로 타입을 변환합니다.
     - null과 undefined는 서로 같습니다.
     - boolean 타입은 Number 타입으로 변환합니다. true는 1, false는 0으로 변환됩니다.
     - string 타입은 Number 타입으로 변환합니다. 문자열이 숫자로 이루어져 있다면 해당 숫자로 변환됩니다. 그렇지 않으면 NaN으로 변환됩니다.
     - object 타입과 symbol 타입은 Number 타입으로 변환합니다. valueOf() 메소드가 숫자를 반환하면 해당 숫자로 변환됩니다. valueOf() 메소드가 숫자가 아니라면 toString() 메소드의 반환값을 다시 Number 타입으로 변환합니다. 그렇지 않으면 NaN으로 변환됩니다.
     - NaN == NaN은 false입니다.
- `===` 는 엄격한 같음(strict equality)으로 두 값이 같은지 비교합니다. 이때, 형 변환은 일어나지 않고, 둘이 서로 다른 형이면, 둘은 같지 않다고 판단합니다.
- 관련 내용
  - `==` 는 암묵적 형변환이이 일어나는데, 암묵적 형변환이 일어날 것을 모두 기억하거나 예측하는 것이 어렵기 때문에, 의도하지 않은 결과를 얻게 될 가능성이 크고 이로 인해 오류 가능성이 커집니다. 따라서 동등함을 비교하기 위해서 `===` 를 사용하는 것이 좋습니다.
  - 비교 연산 중에 ES6(ECMAScript 2015)에 추가된 `Object.is` 도 있습니다. `+0`, `0`, `NaN`, 비교 이외에는 `===` 연산과 동일한 결과를 줍니다.
    - Object.is(NaN, NaN)은 true가 아닌 false를 반환합니다.
    - Object.is(+0, -0)은 false가 아닌 true를 반환합니다.
  - 객체간 비교할 경우 객체 안의 내용이 같더라도 참조형이기 때문에 `==`, `===`, `Object.is` 로 비교하면 `false`로 판단합니다. 따라서 `JSON.stringify` 로 객체 안의 내용을 문자열로 변환한 후 비교 하거나 순서가 보장되지 않는 값이라면, 정렬 후 비교 합니다.
</details>

<details>
  <summary>()</summary>
  <br />
  
  -
</details>
