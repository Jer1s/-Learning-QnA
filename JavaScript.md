<details>
  <summary>JavaScript란? (8)</summary>

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
  <summary>JIT 컴파일 프로그래밍 언어란? (2(3))</summary>

  - `JIT compiler` Just-In-Time의 준말으로, 런타임 시점에 코드를 컴파일하는 방식을 말합니다.
  - `JIT compile programing language` 
    - JIT 컴파일러를 사용한 언어
    - 이를 통해 실행 속도를 향상시키고, 메모리 사용량을 줄일 수 있습니다.
    - 대표적인 JIT 컴파일 프로그래밍 언어로는 Java, C#, JavaScript(V8 엔진), Python(PyPy) 등이 있습니다.
</details>

<details>
  <summary>JavaScript에서 Semi colon의 의미를 설명해주세요. (3)</summary>

  - 한 문장 맨 끝에 세미콜론(;)을 붙여 문장을 구분합니다.
  - Javascript는 코드를 해석하는 과정에서 상황에 따라 자동으로 세미콜론을 추가해주는 규칙이 있습니다.
  - 필요한 경우에만 사용하는 사람도 있고 반드시 사용하는 사람이 있습니다.
</details>

<details>
  <summary>JavaScript에서 comment를 다는 법을 설명해주세요. (1)</summary>

  - `//` 뒤, `/* */` 사이의 내용은 실행되지 않습니다.
</details>

<details>
  <summary>변수 선언자(variable declarator)은 어떤 것이 있나요? (3(6))</summary>

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

  - JavaScript 식별자는 '문자(a-z,A-Z)', '밑줄(\_)' 혹은 '달러 기호($)'로 시작해야 합니다.
  - 두 번째 글자부터는 '숫자(0-9)'도 쓸 수 있습니다.
  - 대문자와 소문자를 구분합니다.
  - 예약어(Reserved word)는 사용할 수 없습니다. (Ex. if, for, let, this, ...)
</details>

<details>
  <summary>Variable naming rule 중 선택 규칙을 설명해주세요. (3)</summary>

  - 추상화와 구체화가 적당한 이름이 좋습니다.
  - 이름에 의미를 담는 것이 좋습니다.
  - 'camelCase'로 쓰는 것이 좋습니다.
</details>

<details>
  <summary>function 선언, 호출 방법을 설명해주세요. (2)</summary>

  - `function my_func(parameters) {statements}` 형태로 선언합니다.
  - `my_func(arguments);` 형태로 호출합니다.
</details>

<details>
  <summary>Parameter란? (4)</summary>

  - 함수를 호출할 때 괄호 안에 parameter를 넣어 전달하면 함수 내부에서 사용할 수 있습니다.
  - 전달되지 않은 parameter는 undefined 값으로 설정됩니다.
  - Default parameter로 전달되지 않았을 때의 기본값을 설정할 수 있습니다.
  - Default parameter는 뒷쪽에 쓰는 것이 좋습니다.
</details>

<details>
  <summary>Return이란? (1)</summary>

  - 함수가 실행된 자리에 값을 전달할 수 있게 해줍니다.
</details>

<details>
  <summary>JavaScript에서 ==, ===의 차이점은? (3)</summary>

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
  <summary>객체란? (1)</summary>
  
```jsx
{
  property_name: property_value,
  // ...
}
</details>

<details>
  <summary>프로퍼티에 대해 설명해주세요. (5(3))</summary>
  
  - 프로퍼티 네임을 `key`라고도 합니다.
  - 프로퍼티 네임은 문자열이지만 따옴표를 생략해도 JavaScript가 암묵적으로 문자열로 형변환합니다.
  - 프로퍼티 네임 주의 사항
    - 첫 번째 글자는 반드시 문자, 밑줄(_), 달러 기호($) 중 하나로 시작해야 합니다.
    - 띄어쓰기를 쓰면 안됩니다.
    - 하이픈(-)을 쓰면 안됩니다.
  - 주의 사항에 어긋나는 프로퍼티 네임은 따옴표로 감싸줘야 합니다.
  - 프로퍼티 밸류에는 객체를 포함한 모든 데이터 타입의 값을 쓸 수 있습니다.
</details>

<details>
  <summary>객체에서 데이터에 접근하는 법은? (4(1))</summary>
  
  - `object.key`: 점 표기법
    - 따옴표를 생략할 수 없는 키 값으로는 접근할 수 없습니다.
  - `object['key']`: 대괄호 표기법
  - key와 대응되는 value를 리턴합니다.
  - 존재하지 않는 key 값을 넣으면 undefined를 리턴합니다.
</details>

<details>
  <summary>객체를 다루는 방법은? (3(5))</summary>
  
  - `object.key = value;`
    - 존재하는 key 값일 경우 새로 입력한 value 값을 할당합니다.
    - 존재하지 않는 key 값일 경우 새로운 key-value 쌍을 생성합니다.
  - `delete object.key;`: 객체 내의 키-밸류 쌍을 삭제합니다.
  - `key in object`
    - 존재하는 key 값일 경우 true를 리턴합니다.
    - 존재하지 않는 key 값일 경우 false를 리턴합니다.
    - 예기치 않게 프로퍼티 밸류 값에 undefined가 할당되더라도 존재하는 프로퍼티 네임이라고 확인할 수 있습니다.
</details>

<details>
  <summary>객체의 메서드란? (1)</summary>
  
  - 프로퍼티 밸류가 함수인 키
</details>

<details>
  <summary>객체의 메서드의 장점은? (3)</summary>
  
  - 다른 함수의 이름 중복을 피할 수 있습니다.
  - 객체에 집중해서 함수의 동작 부분을 작성할 수 있습니다.
  - 객체의 고유한 동작으로 구분할 수 있기 때문에 좀 더 의미 있는 코드로 활용이 가능합니다.
</details>

<details>
  <summary>for...in 반복문에 대해서 설명해주세요. (4(3))</summary>
  
```jsx
for (variable in object)
  statement
  - `variable`: 매 반복마다 키 값을 문자열로 할당 받습니다.
  - `statement`: `object[variable]`로 value값에 접근할 수 있습니다.
  - 정수형 프로퍼티 네임을 사용할 때
    - 정수형 프로퍼티 네임을 오름차순으로 먼저 정렬하고 나머지 프로퍼티들은 추가한 순서대로 정렬하는 특징이 있습니다.
    - 이러한 이유로 정수형 프로퍼티는 일반적으로 사용되지 않습니다.
</details>

<details>
  <summary>Date 객체란? (2)</summary>
  
  - 내장 객체(Standard built-in objects) 중 하나로 1970년 1월 1일 UTC(협정 세계시) 자정과의 시간 차이를 밀리초로 나타내는 정수 값을 담습니다.
  - [Date - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) 참조
</details>

<details>
  <summary>배열(Array)란? (4)</summary>
  
```jsx
let arr = [
  element1,
  // ...
  elementN
];
  - `arr[index]`: index(0부터 시작하는 정수 값)을 활용하여 element에 접근할 수 있습니다.
  - element에 array 값을 넣으면 다차원 배열을 활용할 수 있습니다.
  - 특별한 객체의 한 종류입니다.
</details>

<details>
  <summary>배열의 메서드에 대해 설명해주세요. (10(10))</summary>
  
  - `length`: 배열의 길이를 리턴합니다.
  - `splice(start[, deleteCount[, item1[, item2[, ...]]]]`: 배열의 여러 요소를 수정/삭제하고 삭제된 요소들을 포함한 배열을 리턴합니다.
    - `start`: 배열의 변경을 시작할 인덱스
    - `deleteCount`: 배열에서 제거할 요소의 수
    - `itemN`: 배열에 삭제한 위치에 추가할 요소
  - `shift()`: 배열의 첫 번째 요소를 제거하고 리턴합니다.
    - 빈 배열이 아니라면 배열의 길이가 줄어듭니다.
  - `pop()`: 배열 끝에서부터 요소를 제거합니다.
  - `unshift(element)`: 배열 앞에 요소를 추가합니다.
  - `push(element)`: 배열 끝에 요소를 추가합니다.
  - `indexOf(element)`: 배열 안 요소의 인덱를 리턴합니다.
    - element가 array에 포함되어 있다면 item이 있는 인덱스를 리턴합니다.
    - element가 array에 포함되어 있지 않다면 -1을 리턴합니다.
    - 여러 번 포함되어 있으면 처음 발견된 인덱스를 리턴합니다.
    - `lastIndxOf(element)`: 여러 번 포함되어 있을 때 마지막 인덱스를 리턴합니다
  - `includes(element)`: element가 array에 포함되어 있는지 여부를 boolean 값으로 리턴합니다.
  - `reverse()`: 배열의 순서를 뒤집습니다.
  - [Array - JavaScript | MDN](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array) 참조
</details>

<details>
  <summary>for..of 반복문에 대해 설명해주세요. (3)</summary>

```jsx
for (variable of array)
  statement

```
  - `variable`: 매 반복마다 element를 할당받습니다.
  - `for...in` 문도 배열에 쓸 수 있지만 배열의 메서드나 프로퍼티 등이 의도하지 않게 variable에 할당될 수 있으므로 배열에는 `for...of` 문을 쓰는 것이 좋습니다.
</details>

<details>
  <summary>숫자 표기법에 대해 설명해주세요. (4)</summary>
  
  - `NeM`: N * 10M의 지수 표기법입니다.
  - `0xN`: 16진법의 표기법입니다.
  - `0oN`: 8진법의 표기법입니다.
  - `0bN`: 2진법의 표기법입니다.
</details>

<details>
  <summary>숫자형 메서드에 대해 설명해주세요. (4)</summary>
  
  - `toFixed(N)`: 소수점 N번째 자리까지 표현된 값을 문자열로 리턴합니다.
  - `tostring(N)`: N진법으로 표현된 값을 문자열로 리턴합니다.
  - `Number` 함수로 형 변환을 해도 되지만 숫자로 된 문자열 앞에 더하기(+) 기호를 붙이면 숫자형으로 형변환됩니다.
  - 정수에 그대로 숫자형 메소드를 쓰면 소수점으로 인식하여 오류가 나기 때문에 온점을 두 번(..) 쓰거나 숫자를 괄호로 감싸주거나 숫자를 변수에 할당한 후 써야합니다.
</details>

<details>
  <summary>Math 객체의 메서드를 설명해주세요. (9)</summary>
  
  - `Math.abs(N)`: 절댓값을 리턴합니다.
  - `Math.max(N1, N2, ...)`: 최댓값을 리턴합니다.
  - `Math.min(N1, N2, ...)`: 최솟값을 리턴합니다.
  - `Math.pow(N, M): NM 값을 리턴합니다.
  - `Math.sqrt(N): N의 제곱근을 리턴합니다.
  - `Math.round(N)`: N의 올림 값을 리턴합니다.
  - `Math.ceil(N)`: N의 버림 값을 리턴합니다.
  - `Math.random()`: 0 이상 1 미만의 랜덤한 값을 리턴합니다.
</details>

<details>
  <summary>문자열 메서드를 설명해주세요. (9(6))</summary>
  
  - `string.length`: 문자열의 길이를 리턴합니다.
  - `string[N]`: 해당 인덱스의 문자를 리턴합니다.
  - `string.indexof('a')`: 해당 문자를 갖는 첫 번째 인덱스를 리턴합니다.
  - `string.lastIndexof('a')`: 해당 문자를 갖는 마지막 인덱스를 리턴합니다.
  - `string.toUpperCase()`: 문자열을 모두 대문자로 변환하여 리턴합니다.
  - `string.toLowerCase()`: 문자열을 모두 소문자로 변환하여 리턴합니다.
  - `string.trim()`: 양 쪽 끝의 공백을 제거한 문자열을 리턴합니다.
  - `string.slice([start], [end])`
    - start index부터 end index 직전까지의 범위의 문자열을 리턴합니다.
    - end를 생략할 경우 start index부터 끝까지의 범위의 문자열을 리턴합니다.
    - start, end를 생략할 경우 문자열을 그대로 리턴합니다.
  - 배열과 다른 점
    - typeof 연산자의 리턴 값이 다릅니다.
    - 한 배열과 한 문자열의 내용이 같더라도 일치 비교, 동등 비교에서 false가 출력됩니다.
    - 문자열은 배열과 다르게 바뀔 수 없는(immutable) 자료형입니다.
</details>

<details>
  <summary>기본형이란? (1(5))</summary>
  
  - 기본형(primitive type)은 변수에 할당할 때 메모리에 값을 그대로 저장하는 변수 타입입니다.
    - Boolean
    - number
    - String
    - null
    - undefined
</details>

<details>
  <summary>참조형이란? (1(3))</summary>
  
  - 참조형(reference type)이란 변수에 할당할 때 메모리의 주소 값을 저장하는 변수 타입입니다.
    - array
    - function
    - object
</details>

<details>
  <summary>참조형 복사에 대해 설명해주세요. (4)</summary>
  
  - 참조형 변수를 다른 변수에 할당하면 주소값만 복사됩니다.
  - `array2 = array1.slice();`: 배열의 실제 값을 복사합니다.
  - `Object.assing(target, source)`: source object의 모든 프로퍼티를 복사해 target object에 붙여넣습니다. 그 후 대상 객체를 반환합니다.
  - 객체 안에 객체가 있는 경우 `Lodash`나 `Immer`같은 라이브러리를 사용하거나(패키지를 설치해야함), `JSON.stringify()`와 `JSON.parse()` 함수를 이용하여 객체를 문자열로 변환한 후 다시 객체로 변환하는 방법(느림), 또는 재귀 함수를 이용한 깊은 복사를 하여(직접 구현해야함) 깊은 복사할 수 있습니다.
</details>

<details>
  <summary>const 키워드로 변수를 선언해야 하는 이유에 대해 설명해주세요. (4)</summary>
  
  - 몇몇 스타일 가이드에서는 변수를 const 키워드로 선언하라고 권장하고 있습니다.
  - 변수의 재할당을 방지하여 코드의 일관성과 안정성이 올라갑니다.
  - 변수가 의미론적으로 상수라면 이름을 대문자로, 두 단어 사이는 밑줄로 구분하여 작성하고, 의미론적으로 변수라면 이름을 camelCase로 작성하여 구분 짓는 게 좋습니다.
  - const 키워드로 참조형 변수를 선언해도 주소값만 저장되기 때문의 객체 내부는 변동될 수 있습니다.
</details>

<details>
  <summary></summary>
  
  - 
</details>

<details>
  <summary></summary>
  
  - 
</details>

<details>
  <summary></summary>
  
  - 
</details>
