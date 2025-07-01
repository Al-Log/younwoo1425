## 📘 문제 이름

- 🧩 난이도:
- 🛠 사용 언어:
- [문제링크](https://school.programmers.co.kr/learn/courses/30/lessons/181920)

---

### 🧠 문제 설명

## 정수 start_num과 end_num이 주어질 때, start_num부터 end_num까지 1씩 증가하는 정수들을 차례대로 담은 리스트를 반환하는 문제

### 💡 아이디어

아직 다른 아이디어는 잘 떠오르지 않음

---

### 배운 것, 느낀 점, 아직 이해되지 않은 점 (선택)

처음 C++ 입출력 방식이 헷갈려서 scanf, cin, printf, cout을 혼용했는데 이 문제에서는 전혀 쓸 필요가 없었다는 걸 깨달음.

함수가 직접 start_num, end_num 값을 받기 때문에 입출력 코드는 쓰면 안 된다는 걸 느꼈다.

vector 사용법, for문 반복 방식 등 아주 기초지만 확실히 이해하게 된 문제.

---

### 다른 사람의 풀이

#include <vector>
#include <numeric> // iota
using namespace std;

vector<int> solution(int start, int end) {
vector<int> answer(end - start + 1);
iota(answer.begin(), answer.end(), start); // 자동으로 순차값 채움
return answer;
}
