# [1. Two Sum](https://leetcode.com/problems/two-sum/)

**난이도**: Easy
**유형**: Array, Hash Table

## 문제 요약
정수 배열 `nums`와 목표값 `target`이 주어졌을 때, 두 수의 합이 `target`이 되는 두 인덱스를 반환한다.

## 접근법
1. Brute force: 이중 반복문으로 모든 쌍을 확인 → O(n²)
2. HashMap 최적화: 배열을 한 번 순회하면서, 현재 값의 보수(`target - nums[i]`)가 이미 map에 있는지 확인 → O(n)

## 시간/공간 복잡도
- Time: O(n)
- Space: O(n)

## 배운 점
- `Map.containsKey` / `Map.get`을 이용한 O(1) 조회 패턴
- Java에서 배열을 리턴할 때 `new int[] { a, b }` 문법
