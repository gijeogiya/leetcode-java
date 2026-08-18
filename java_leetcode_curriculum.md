# Java LeetCode 16주 커리큘럼 (빅테크 코딩테스트 대비)

## 배경
- 목표 페이스: 주 3문제
- 목표: 빅테크 코딩테스트/기술 인터뷰 대비

## 커리큘럼 설계 원칙
- 1~2주차: 쉬운 난이도로 Java 컬렉션(HashMap, ArrayList, StringBuilder 등) 손에 익히기
- 3주차 이후: Blind 75 / NeetCode 150 기준으로 빅테크 기출 빈도가 높은 유형 순서대로 진행
- 매주 3문제 = Easy 1~2 + Medium 1~2 비율로 구성 (뒤로 갈수록 Medium/Hard 비중 증가)

## 주차별 계획

| 주차 | 테마 | 문제 (난이도) | Java 학습 포인트 |
|---|---|---|---|
| 1 | 배열/해시 기초 | Two Sum (E) · Contains Duplicate (E) · Valid Anagram (E) | HashMap, HashSet 기본 사용법 |
| 2 | 배열/문자열 | Best Time to Buy/Sell Stock (E) · Valid Palindrome (E) · Group Anagrams (M) | StringBuilder, Arrays.sort, Collections |
| 3 | Two Pointer | Container With Most Water (M) · 3Sum (M) · Longest Substring w/o Repeating Characters (M) | 포인터 두 개 다루는 패턴을 Java로 재구현 |
| 4 | Sliding Window | Longest Repeating Character Replacement (M) · Permutation in String (M) · Minimum Window Substring (H) | int[26] 배열 카운팅, 윈도우 축소/확장 |
| 5 | Stack | Valid Parentheses (E) · Min Stack (M) · Evaluate Reverse Polish Notation (M) | Deque를 Stack으로 활용 |
| 6 | Linked List 기초 | Reverse Linked List (E) · Merge Two Sorted Lists (E) · Linked List Cycle (E) | 커스텀 클래스(ListNode) 다루기, null 처리 |
| 7 | Linked List 심화 | Remove Nth Node From End of List (M) · Reorder List (M) · Add Two Numbers (M) | Fast/Slow pointer, dummy node 패턴 |
| 8 | Tree 기초 | Invert Binary Tree (E) · Maximum Depth of Binary Tree (E) · Same Tree (E) | 재귀 함수 Java 문법(리턴 타입 명시 등) |
| 9 | Tree/BST 심화 | Validate Binary Search Tree (M) · Kth Smallest Element in a BST (M) · Lowest Common Ancestor of a Binary Search Tree (M) | 재귀 + 클래스 필드 활용 |
| 10 | 백트래킹 | Subsets (M) · Combination Sum (M) · Permutations (M) | List<List<Integer>> 다루기, 재귀 백트래킹 |
| 11 | 그래프 BFS/DFS | Number of Islands (M) · Clone Graph (M) · Course Schedule (M) | Queue(BFS), visited 배열/HashSet |
| 12 | 그래프 심화 | Pacific Atlantic Water Flow (M) · Word Search (M) · Rotting Oranges (M) | 멀티소스 BFS, 2차원 배열 탐색 |
| 13 | DP 기초 | Climbing Stairs (E) · House Robber (M) · Coin Change (M) | 1차원 DP 배열, memoization |
| 14 | DP 심화 | Longest Increasing Subsequence (M) · Unique Paths (M) · Word Break (M) | 2차원 DP, DP + HashSet 조합 |
| 15 | 힙/그리디 | Top K Frequent Elements (M) · Kth Largest Element in an Array (M) · Merge Intervals (M) | PriorityQueue(Comparator) 활용 |
| 16 | 종합/기출 | Trapping Rain Water (H) · LRU Cache (M/H) · 취약 유형 재도전 1문제 | 지금까지 배운 패턴 종합 적용 |

## 학습 전략

1. **1~2주차는 시간 제한 없이** — Java 문법과 씨름하느라 시간이 오래 걸려도 정상. 여기서 익힌 문법이 이후 속도를 좌우함.
2. **3주차부터는 40분 타임박스** — Python으로는 바로 풀리는 문제도 Java 컴파일 에러/타입 이슈로 막힐 수 있으니, 막히면 답을 보되 반드시 손으로 다시 타이핑.
3. **주말에 1문제씩 "말로 설명하며 풀기"** — 빅테크 인터뷰는 설명력이 중요하니, 풀이 과정을 소리 내어 설명하는 연습을 곁들이면 좋음.
4. **8주차 정도에 한 번 중간 점검** — 유독 느렸던 유형(예: DP, 그래프)이 있으면 15~16주차 비중을 그쪽으로 조정.
5. 10주차(백트래킹) 이후부터는 Medium 난이도가 계속 나오니, 페이스가 힘들면 주 3문제를 2 Medium + 1 Easy 복습으로 조정 가능.
