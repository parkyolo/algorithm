## AC

### 문제
https://www.acmicpc.net/problem/5430  
선영이는 주말에 할 일이 없어서 새로운 언어 AC를 만들었다. AC는 정수 배열에 연산을 하기 위해 만든 언어이다. 이 언어에는 두 가지 함수 R(뒤집기)과 D(버리기)가 있다.

함수 R은 배열에 있는 수의 순서를 뒤집는 함수이고, D는 첫 번째 수를 버리는 함수이다. 배열이 비어있는데 D를 사용한 경우에는 에러가 발생한다.

함수는 조합해서 한 번에 사용할 수 있다. 예를 들어, "AB"는 A를 수행한 다음에 바로 이어서 B를 수행하는 함수이다. 예를 들어, "RDD"는 배열을 뒤집은 다음 처음 두 수를 버리는 함수이다.

배열의 초기값과 수행할 함수가 주어졌을 때, 최종 결과를 구하는 프로그램을 작성하시오.

### 풀이
- 입력 배열을 ","으로 split해서 배열 형태로 만듦
- "R"일 때 reversed 변수를 반전
- "D"일 때
    - nums_array가 비어있으면 'error' 반환
    - 비어있지 않고 reversed == True이면 맨 뒤의 원소를 pop
    - 비어있지 않고 reversed == False이면 맨 앞의 원소를 pop