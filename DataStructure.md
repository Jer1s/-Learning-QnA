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

- Argument가 특정 값 또는 무한대로 향하는 경향이 있을 때 함수의 동작 범위 설명하는 수학적 표기법입니다.
- 어떤 함수 `f(n)`의 Big-O notation이 `O(g(n))`이라는 것은, n의 값이 일정 수준을 넘어가면 그 이상의 어떤 n을 대입하여도 `|f(n)| < c*g(n)`을 만족하는 양의 실수 c가 존재한다는 뜻입니다.
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
<summary>알고리즘이란? (2)</summary>
<br>

- `알고리즘(algorithm)` 유한하게 연속적인 정밀한 명령
- 문제를 효율적이게 해결하는 것이 좋은 알고리즘이다.
</details>

<details>
<summary>선형 탐색 알고리즘(linear search algorithm)이란? (2)</summary>
<br>

- 한쪽 끝에서 시작하여 원하는 요소를 찾을 때까지 목록의 각 요소를 검색하는 알고리즘
- Performance
  - Worst-case time complexity: O(n)
  - Best-case time complexity: O(1)
  - Average time complexity: O(n)
  - Worst-case space complexity: O(1)
  - Best-case space complexity: O(1)
  - Average space complexity: O(1)
</details>

<details>
<summary>이진 탐색 알고리즘(Binary search algorithm)이란? (3)</summary>
<br>

- 정렬된 배열에서 탐색 범위를 절반씩 줄여 나가면서 원하는 요소를 찾는 알고리즘
- Process
  1.  정렬된 배열에서 원하는 요소와 배열의 중간 요소를 비교합니다.
  2. 동일하지 않으면 대상이 존재할 수 없는 배열의 절반이 제거되고 나머지 배열 절반에서 검색이 계속됩니다.
  3. 반으로 줄어든 배열에서 대상 값을 찾을 때까지 이 작업을 반복합니다.
- Performance
  - Worst-case time complexity: O(log n)
  - Best-case time complexity: O(1)
  - Average time complexity: O(log n)
  - Worst-case Space complexity: O(1)
  - Best-case Space complexity: O(1)
  - Average Space complexity: O(1)
</details>

<details>
<summary>선택 정렬 알고리즘(Selection sort algorithm)이란? (2)</summary>
<br>

- Process
  1. 주어진 배열의 요소 중 최솟값을 찾습니다.
  2. 그 값을 맨 앞에 위치한 값과 교체합니다.
  3. 맨 처음 위치를 제외한 나머지 배열에서 같은 방법을 반복합니다.
- Performance
  - Worst-case time complexity: O(n^2)
  - Best-case time complexity: O(n^2)
  - Average time complexity: O(n^2)
  - Worst-case Space complexity: O(1)
  - Best-case Space complexity: O(1)
  - Average Space complexity: O(1)
</details>

<details>
<summary>삽입 정렬 알고리즘(Insertion sort algorithm)이란? (2)</summary>
<br>

- Process
  1. 배열의 두 번째 요소부터 시작합니다. (첫 번째 요소는 정렬이 되어있는 상태이기 때문에)
  2. 그 요소의 왼쪽에 위치한 부분 배열과 비교하여, 그 요소를 부분 배열 속에 삽입할 위치로 이동시킵니다.
  3. 나머지 배열에서 같은 방법을 인덱스 순서대로 반복합니다.
- Performance
  - Worst-case time complexity: O(n^2)
  - Best-case time complexity: O(n)
  - Average time complexity: O(n^2)
  - Worst-case Space complexity: O(1)
  - Best-case Space complexity: O(1)
  - Average Space complexity: O(1)
</details>

<details>
<summary>자료 구조(Data structuer)란?</summary>
<br>

- 데이터의 효율적인 접근 및 조작을 가능하게 해주는 저장 및 관리 방식
</details>

<details>
<summary>배열(list)란?</summary>
<br>

- 메모리 상에 같은 타입의 자료가 연속적으로 저장되는 자료 구조
</details>

<details>
<summary> </summary>
<br>

- 
</details>

<details>
<summary>튜플(Tuple)이란?</summary>
<br>

- 둘 이상의 자료형을 묶음으로 다루는 자료 구조
</details>

<details>
<summary>연결 배열(Linked list)이란? (2)</summary>
<br>

- 자료와 다음 노드를 가리키는 참조값으로 구성된 노드를 단위로 하는 잘교 구조
- 원형 연결, 이중 연결 등의 연결 리스트도 있습니다.
</details>

<details>
<summary>해시 테이블(Hash table)이란? (4)</summary>
<br>

- 키를 값에 매핑할 수 있는 자료 구조
- 해시 함수를 사용하여 해시 코드로 인덱싱합니다.
- 조회 중에 키가 해시되고 결과 해시는 해당 값이 저장된 위치를 나타냅니다.
- 해시 맵(Hash map)이라고도 부르는데, Java에서 둘의 차이점은 있습니다.
</details>

<details>
<summary>스택(stack)이란? (4)</summary>
<br>

- Push, Pop 두 가지 주요 연산으로 구성된 선형 자료 구조
- `Push` 컬렉션에 요소를 추가
- `Pop` 아직 제거되지 않은 가장 최근에 추가된 요소를 제거
- 가장 최근에 저장된 데이터를 먼저 제거해야 이전에 저장된 데이터에 접근할 수 있습니다.
</details>

<details>
<summary>큐(Queue)란? (2)</summary>
<br>

- 먼저 저장된 데이터가 먼저 나오는 FIFO(First in First Out) 형식의 선형 자료 구조
- 스택과 반대되는 개념입니다.
</details>

<details>
<summary>덱(Deck)이란? (2)</summary>
<br>

- 시작과 끝에서 넣기와 빼기를 할 수 있는 형식의 선형 자료 구조
- 큐와 스택을 합친 형태입니다.
</details>

<details>
<summary>그래프(Graph)란? (3)</summary>
<br>

- vertex와 edge로 구성된 비선형 자료 구조
- edge의 방향성 유무에 따라 directed graph, undirected graph로 나뉩니다.
- weight의 유무에 따라 weighted graph, unweighted graph로 나뉩니다.
</details>

<details>
<summary>트리(Tree)란? (4)</summary>
<br>

- 연결된 노드 집합이 있는 계층적 비선형 자료 구조
- 자식 노드는 여러 개일 수 있지만, root node를 제외하고는 정확히 하나의 부모 노드에 연결해야 합니다.
- 이진 트리(Binary tree)
  - 각 노드에 최대 두 개의 자식이 있는 트리 구조
- 이진 힙(Binary heap)
  - 부모 노드와 자식 노드의 키 값 사이의 대소관계가 항상 일정한 이진 트리
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
