# [2. Contains Duplicate](https://leetcode.com/problems/contains-duplicate/)

**난이도**: Easy
**유형**: Array, Hash Table

## 문제 요약
정수 배열 `nums`와가 주어졌을 때, 중복된 숫자 존재 유무(`true` 또는 `false`)를 반환한다.

## 접근법
1. HashMap 최적화: 배열을 한 번 순회하면서, 현재 값이 이미 map에 있는지 확인 → O(n)

## 시간/공간 복잡도
- Time: O(n)
- Space: O(n)

## 배운 점
### Java 문법
#### HashMap
- key와 value 구성 단위의 자료구조
- key가 곧 주소여서 key를 쿼리시, 시간 복잡도가 상수이다. O(1)
- 선언: Map<Integer, Integer> seen = new HashMap<>();
- key가 있는지 조회: seen.containsKey(key);
- 값 넣기: seen.put(key, value);
- 값 확인: seen.get(key);
