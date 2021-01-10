# 코딩 꿀팁 #


1. 이진 탐색 문제는 입력 데이터가 많거나, 탐색 범위가 매우 넓은 편이다. => 데이터의 크기가 1000만개 이상이거나 탐색 범위의 크기가 1000억 이상리면 이진 탐색 알고리즘을 의심하자.
- input()으로 받으면 동작 속도가 느리므로 sys라이브러리를 이용하자

import sys 

input_data = sys.stdin.readline().rstrip()

print(input_data)


2. 다이나믹 프로그래밍을 사용할 수 있는 경우
- 큰 문제를 작은 문제로 나눌 수 있다.
- 작은 문제에서 구한 정답은 그것을 포함하는 큰 문제에서도 동일하다.



3. 최단경로 알고리즘
- 다익스트라 : 한 지점에서 다른 지점으로 가는 최단 경로 , 시간복잡도 = O(ElogV) (E=간선의 개수,V=노드의 개수)
- 플로이드 워셜 : 모든 지점에서 다른 모든 지점까지의 최단 경로 , 시간복잡도 = O(N^3)


4. 각 노드간의 거리(비용)이 모두 1일때는 BFS를 고려하자

5. BFS에서 최단경로상에 존재하는 노드를 출력하고 싶을 때는 역추적을 하자.
- 즉 현재 노드는, 이전 노드에 연결돼있다는 개념을 이용
