## 부분수열의 합
### 문제
https://www.acmicpc.net/problem/1182  
N개의 정수로 이루어진 수열이 있을 때, 크기가 양수인 부분수열 중에서 그 수열의 원소를 다 더한 값이 S가 되는 경우의 수를 구하는 프로그램을 작성하시오.
### 풀이
- 부분수열을 구하기 위해 백트래킹 사용
- 부분수열의 길이가 0보다 크고, 수열의 원소를 더한 값 sum_이 S가 되는 경우 cnt += 1