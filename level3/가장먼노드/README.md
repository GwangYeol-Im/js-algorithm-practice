## N으로 표현

- [출처](https://programmers.co.kr/learn/courses/30/lessons/49189)

### 입력

- n - 노드 개수
- vertex - 연결된 노드 정보를 담은 2차원 배열

### 출력

- 1번 노드부터 가장 거리가 먼 노드의 개수

### 아이디어

- 간선 간 거리가 같아 다익스트라가 아닌 BFS로 해결
- 초반에 graph\[n\]\[n\]을 만들어 놓고 연결된 노드라면 1, 나머지는 0을 부여 -> seg fault 뜸
- 두번쨰 시도 - graph\[n\] 안에 빈 배열을 만들어주고 연결된 노드의 정보를 push 했음 -> 성공
