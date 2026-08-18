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
### Java 문법
#### Array
- Array 배열은 공간의 갯수가 정해져 있는 자료구조이다. (선언 시 공간 갯수가 정해짐)
- 선언방법: int arr[] = new int[5];
- 선언 후 대입: arr[1] = 5;
- 선언 후 참조: arr[1] //5
- 길이 출력: arr.length;
- 선언과 합께 대입: int arr[]= {1, 2, 3, 4, 5} //선언과 함꼐 대입시에는 크기는 따로 안적어주어도 그 길이가 정해진다.
- 이중 배열: int[][] arr = new int[3][2];
- 복사: 깊은 복사는 수동으로 for문 돌리면서 값을 대입해주는 방법 밖에 없다.
- 정렬
```java
import java.util.Arrays;
import java.util.Comparator;

public class main {
    public static void main(String[] args) {

        class User {
            private String name;
            private int age;

            User(String name, int age) {
                this.name = name;
                this.age = age;
            }

            public int getAge() {
                return this.age;
            }
            public String getName() {
                return this.name;
            }
        }

        User[] users = {
            new User("홍길동", 30),
            new User("김춘추", 60),
            new User("임꺽정", 30),
            new User("김좌진", 20),
            new User("주몽", 50),
            new User("심사임당", 30),
        };

        Arrays.sort(users, Comparator.comparing(User::getAge)); // 나이순 정렬
        for (User u : users) { System.out.println(u.name + " " + u.age + "세"); } // 출력

        System.out.println("\n");

        Arrays.sort(users, Comparator.comparing(User::getName)); // 이름순 정렬
        for (User u : users) { System.out.println(u.name + " " + u.age + "세"); }

        System.out.println("\n");
       
        Arrays.sort(users, Comparator.comparing(User::getAge).thenComparing(User::getName)); // 먼저 나이순 정렬하고 나이가 같으면 따로 이름순 정렬
        for (User u : users) { System.out.println(u.name + " " + u.age + "세"); }
    }
}
```

### 순열과 조합
#### 순열
```java
public class Main {
    static int[] arr = {1, 2, 3, 4};    // n에 해당하는 배열
    static int[] output;                // r개를 뽑은 배열
    static boolean[] visited;            // 방문 처리 배열
    static int N = 4, R = 3;            // n은 4, r은 3

    public static void main(String[] args) {
        output = new int[R];        // r개를 뽑은 배열 초기화
        visited = new boolean[N];    // 방문 처리 배열 초기화

        ...
    }
}

static void permutation(int depth, int n, int r) {
    // 순열이 완성된 경우
    if(depth == r) {
        System.out.println(Arrays.toString(output));
        return;
    }

    // 0부터 n까지 반복
    for(int i = 0; i < n; i++) {
        // 방문하지 않은 값이면 넣기
        if(!visited[i]) {
            visited[i] = true;    // 방문 처리
            output[depth] = arr[i];    // 현재 depth를 인덱스로 사용
            permutation(depth + 1, n, r);    // depth + 1를 전달
            visited[i] = false; // 다음 순열을 뽑기위해 방문처리 제거
        }
    }
}
```
#### 조합
```java
        for(int i=0; i<nums.length-1; i++){
            for(int j=i+1; j<nums.length; j++){
            }
        }
```
