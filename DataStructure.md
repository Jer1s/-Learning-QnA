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
<summary>스토리지(Storage)란? (4)</summary>
<br>

- 데이터가 장기적으로 보존되는 곳
- 스토리지는 컴퓨터가 꺼져도 데이터가 유지됩니다.
- 읽기 및 쓰기 속도가 메모리에 비해 더 느립니다.
- 하드 디스크 드라이브(HDD), 솔리드 스테이트 드라이브(SSD) 등이 대표적인 예입니다.
</details>

<details>
<summary>메모리(Memory)란? ()</summary>
<br>

- 데이터가 임시로 저장되는 곳
- 읽기 및 쓰기 속도가 스토리지에 비해 더 빠릅니다.
- 자료 구조는 데이터를 메모리에서 잘 사용하도록 하는 게 목적입니다.
- 컴퓨터 메모리는 RAM을 사용합니다.
</details>

<details>
<summary>RAM이란? (4)</summary>
<br>

- RAM(Random Access Memory)은 컴퓨터에서 사용되는 주기억장치 중 하나로, CPU가 빠르게 접근할 수 있는 고속의 메모리입니다.
- RAM은 컴퓨터가 작업할 때 필요한 데이터와 프로그램 코드를 저장하며, 컴퓨터가 실행 중인 프로그램이 필요로 하는 모든 데이터를 RAM에 로드하여 작업을 처리합니다.
- RAM은 데이터를 랜덤한 위치에 저장할 수 있으므로, 컴퓨터가 데이터를 읽거나 쓰는 데 걸리는 시간이 매우 빠릅니다.
- RAM은 휘발성 메모리(Volatile Memory)로서 컴퓨터가 꺼지거나 재부팅 될 경우에 저장된 데이터가 모두 소멸됩니다.
</details>

<details>
<summary>RAM의 cell에 대해서 설명해주세요. (3)</summary>
<br>

- 데이터를 저장할 수 있는 일정한 cell로 나눠져 있습니다.
- 각 cell은 자신만의 주소가 있습니다.
- cell-size는 8-bit, 16-bit, 32-bit, 64-bit 등 다양한 크기로 존재합니다. 8-bit가 주로 사용됩니다.
</details>

<details>
<summary>Random access란? (2)</summary>
<br>

- 저장 위치를 알면 접근할 때 항상 일정한 시간이 걸리는 것
- 메모리에 저장한 데이터에 접근할 때의 시간 복잡도는 O(1)입니다.
</details>

<details>
<summary>레퍼런스란? (2)</summary>
<br>

- 레퍼런스(Reference)는 데이터에 접근하게 해주는 값입니다.
- 해당 데이터의 메모리 주소(Address) 값을 갖거나, 오프셋(offset)을 이용해 데이터를 가리키는 값을 갖을 수 있습니다.
</details>

<details>
<summary>Aliasing이란? (2)</summary>
<br>

- 여러 변수가 같은 메모리를 가리키는 것
- 각 변수를 다른 변수에 대한 alias라고 합니다.
</details>

<details>
<summary>Algorithmic paradigm이란?</summary>
<br>

- 알고리즘 클래스 설계의 기초가 되는 일반화된 모델
</details>

<details>
<summary>Algorithmic paradigm의 종류 (16)</summary>
<br>

- `General`
  - Brute-force search
  - Divide and conquer
  - Dynamic programming
  - Greedy algorithm
  - Backtracking
  - Branch and bound
  - Recursion
  - Prune and search
- `Parameterized complexity` 파라미터들과 관련된 어려운 계산 문제에 초점을 둔 알고리즘 패러다임
  - Kernelization
  - Iterative compression
- `Computational geometry` 기하학 알고리즘 패러다임
  - Sweep line algorithm
  - Rotating calipers
  - Randomized algorithm
</details>

<details>
<summary>Brute-force란? (1)</summary>
<br>

- 가능한 모든 경우의 수를 시도하는 알고리즘 패러다임
</details>

<details>
<summary>Brute-force의 장단점, 의의 (3)</summary>
<br>

- 장점: 직관적이고, 명확하고, 확실하게 답을 찾을 수 있다.
- 단점: 비효율적이다.
- 의의: 효율적인 알고리즘을 찾는 과정의 출발점 역할을 한다.
</details>

<details>
<summary>Divide and Conquer란? (4)</summary>
<br>

- `Divide and Conquer` 문제를 작은 문제로 분할하여 문제를 해결하는 알고리즘 패러다임
	- `divide` 문제를 두 개 이상의 부분 문제로 재귀적으로 분류하는 과정
  - `conquer` 문제가 직접 해결될 수 있을 정도로 간단해진 부분 문제의 솔루션을 구하는 과정
  - `combine` 부분 문제에 대한 솔루션을 결합하여 원래 문제의 답을 구하는 과정
</details>

<details>
<summary>Merge Sort의 과정 (3)</summary>
<br>

- `divide` 배열을 반으로 나눈다.
- `conquer` 왼쪽 배열과 오른쪽 배열을 각각 정렬한다.
- `combine` 정렬된 두 배열을 하나의 정렬된 배열로 합병한다.
</details>

<details>
<summary>Merge sort의 performance (4)</summary>
<br>

- Worst-case time complexity: O(nlog(n))
- Best-case time complexity: O(nlog(n))
- Average time complexity: O(nlog(n))
- Worst-case Space complexity: O(n)
</details>

<details>
<summary>Quick sort의 과정 (3)</summary>
<br>

- `divide` 배열 중 요소 하나를 pivot으로 정하고, pivot 앞에는 pivot보다 값이 작은 모든 요소들이 오고, pivot 뒤에는 pivot보다 값이 큰 모든 원소들이 오도록 분할(partition)합니다.
- `conquer` pivot의 왼쪽 요소들을 모은 배열과 오른쪽 요소들을 모은 배열을 정렬합니다.
- `combine` 없습니다.
</details>

<details>
<summary>Quick sort의 performance (4)</summary>
<br>

- Worst-case time complexity: O(n^2)
- Best-case time complexity: O(nlog(n))
- Average time complexity: O(nlog(n))
- Worst-case Space complexity: O(nN)
</details>

<details>
<summary>Dynamic programming이란? (4)</summary>
<br>

- `Optimal Substructure`, `Overlapping Subproblems`를 가지고 있는 문제를 작은 문제로 분할하여 문제를 해결하는 알고리즘 패러다임
- `Memorization` 또는 `Tabulation` 방법으로 구현할 수 있다.
  - `Optimal Substructure` 부분 문제들의 최적의 답을 이용해서 기존 문제의 최적의 답을 구할 수 있는 구조
  - `Overlapping Subproblems` 부분 문제의 답이 여러 번 재사용될 수 있는 구조
</details>

<details>
<summary>Memorization이란?</summary>
<br>

- 함수 호출 결과를 캐시 메모리에 저장하고 함수가 동일한 입력으로 다시 호출될 경우 캐시 메모리에 저장한 값을 리턴하는 Top-down 접근 방법
</details>

<details>
<summary>Tabulation이란?</summary>
<br>

- 부분 문제의 답을 Table에 저장하고 전체 문제를 해결할 때까지 이러한 결과를 사용하여 더 큰 부분 문제를 해결하는 bottom-up 접근 방법
</details>

<details>
<summary>Memorization, Tabulation의 특징 (14)</summary>
<br>

- `Memorization`
  - Top-down 접근법
  - 부분 문제의 답을 캐싱한다.
  - 재귀적 구현
  - 콜 스택이 계속 쌓이기 때문에 StackOverflow가 발생할 수 있다.
  - 상대적으로 인풋이 작은 문제에 적합하다.
  - 부분 문제가 다른 부분 문제에 overlap될 때 사용한다.
- `Tabulation`
  - Bottom-up 접근법
  - 부분 문제의 답을 Table에 저장한다.
  - 반복문으로 구현
  - 전체 문제에 필요 없는 부분 문제의 계산을 하게 될 수 있다.
  - 상대적으로 인풋이 큰 문제에 적합하다.
  - 부분 문제가 다른 부분 문제에 overlap되지 않을 때 사용한다.
</details>

<details>
<summary>Greedy algorithm이란? (3)</summary>
<br>

- 각 단계에서 국소적으로 최적의 선택을 하는, problem-solving heuristics을 따르는 알고리즘 패러다임
    - `heuristic` 체계적이면서 합리적인 판단을 할 수 없거나 필요하지 않을 때 빠르게 사용할 수 있는 간편추론의 방법
</details>

<details>
<summary>Greedy algorithm으로 풀 수 있는 문제는? (2)</summary>
<br>

- `Optimal Substructure`, `Greedy Choice Property`를 가지고 있는 문제는 Greedy Algorithm으로 최적의 답을 보장할 수 있다.
  - `Greedy Choice Property` globally optimal solution이 locally optimal choice로부터 얻어질 수 있는 특성
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
