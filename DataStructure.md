<details>
<summary>알고리즘의 시간 복잡도란? (3)</summary>
<br>
  
- 알고리즘의 시간 복잡도는 알고리즘이 실행하는 데 걸리는 시간을 입력 길이의 함수로 수량화합니다.
- 실행 시간은 입력 길이의 함수이며 알고리즘이 실행 중인 시스템의 실제 실행 시간이 아닙니다.
- Big O(Ordnung) notation을 통해 표현합니다.
</details>

<details>
<summary>Big O, Big Omega, Big Theta의 차이점은 무엇인가요? (2)</summary>
<br>

- Big O(O)는 시간 복잡도의 상한선, Big Omega(Ω)는 시간 복잡도의 하한선, Big Theta(Θ)는 Big O와 Big Omega 값이 일치할 때를 의미합니다.
- 학계에서 쓰는 Big Theta(Θ) 개념을 산업계에서는 그냥 Big O(O)로 사용합니다.
</details>

<details>
<summary>Big O notation이란? (3)</summary>
<br>

- 인수가 특정 값 또는 무한대로 향하는 경향이 있을 때 함수의 제한 동작을 설명하는 수학적 표기법입니다.
- 어떤 함수 `f(n)`의 Big-O notation이 `O(g(n))`이라는 것은, n의 값이 일정 수준을 넘어가면 그 이상의 어떤 n을 대입하여도 `f(n) < c*g(n)`을 만족하는 상수 c가 존재한다는 뜻입니다.
- `Best-case`, `Worst-case`, `Average(Expected)-case`로 상황별로 나누어서 계산합니다.
</details>

<details>
<summary>공간 복잡도란? (5)</summary>
<br>

- 알고리즘의 공간 복잡도는 알고리즘이 실행하는 데 필요한 공간의 양을 입력 길이의 함수로 수량화합니다.
- 보통 배열의 크기, 예상 동적할당, 재귀함수의 호출 횟수, 스택에 쌓이는 값들의 크기 등이 공간 복잡도에 영향을 미칩니다.
- `Big O notation`을 통해 표현하고, 시간 복잡도와 같은 방법으로 계산합니다.
- `fixed part` 입력 크기와 무관한 코드, 상수, 변수 등의 메모리
- `variable part` 입력 크기에 따라 필요한 공간이 달라지는 메모리
</details>

<details>
<summary>재귀 함수(Recusive function)란?</summary>
<br>

- 자기 자신을 호출하는 함수
</details>

<details>
<summary>재귀적 문제 풀이란? (2)</summary>
<br>

- 재귀적 문제 풀이: 부분 문제(Subprorblem)의 답을 이용해서 기존 문제를 푸는 것
  - 부분 문제(Subproblem): 같은 형태의 더 작은 문제
</details>

<details>
<summary>재귀 함수와 반복문을 비교해주세요. (6)</summary>
<br>

- 반복문으로 풀 수 있는 문제는 재귀 함수로 풀 수 있다.
- 재귀 함수로 풀 수 있는 문제는 반복문으로 풀 수 있다.
- 재귀 함수 호출이 너무 많으면 콜 스택(Call Stack)이 계속해서 쌓이면서 StackOverflowError가 발생한다.
  - 콜 스택(Call Stack): 프로그램이 현재 실행중인 서브루틴에 대한 정보를 저장하는 스택 데이터 구조
  - 파이썬은 콜 스택을 1,000개까지만 허용한다.
- 콜 스택 문제가 일어나지 않을 때, 반복문보다 재귀 함수로 쓰면 코드가 깔끔해지는 문제에는 재귀 함수를 쓰는 것이 좋다.
</details>

<details>
<summary> </summary>
<br>

- 
</details>

<details>
<summary> </summary>
<br>

- 
</details>

<details>
<summary> </summary>
<br>

- 
</details>

<details>
<summary> </summary>
<br>

- 
</details>

<details>
<summary> </summary>
<br>

- 
</details>

<details>
<summary> </summary>
<br>

- 
</details>

<details>
<summary> </summary>
<br>

- 
</details>

<details>
<summary> </summary>
<br>

- 
</details>

<details>
<summary> </summary>
<br>

- 
</details>

<details>
<summary> </summary>
<br>

- 
</details>

<details>
<summary> </summary>
<br>

- 
</details>

<details>
<summary> </summary>
<br>

- 
</details>

<details>
<summary> </summary>
<br>

- 
</details>

<details>
<summary> </summary>
<br>

- 
</details>
