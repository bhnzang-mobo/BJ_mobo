# : 35
R : 82
O : 79
B : 66
. : 46

재귀함수를 이용해 브루트 포스 방법을 이용했다.
문제를 풀어나가면서 현재 R,B의 위치를 잡고
한번 움직일 때 마다 현재 블록에서 R,B의 위치를 보존하기위해
Restore함수를 이용해 복원해주었다.

4가지 경우 left,right,up,down의 모든 경우를 판단하며
Count변수를 전달해 10초과인경우 return.
모든 경우의수를 탐색해 골이 발생한 경우,
골이 발생했을 때 ans값을 Count변수를 이용해 갱신한다.

결과값은 현재 ans 값을 반환.