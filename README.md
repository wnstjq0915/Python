# Python

## 함수
### 예시
- 문제
3명이서 인당 5조각의 피자를 먹을 때  
n개의 피자조각이 주어지면  
몇 개의 피자조각이 남는지
```python
def pizza_mukbang(n):
  # 세 명이서 먹을 수 있는 피자조각
  three_people_pizza = 3 * 5

  # 답 계산
  answer = n - three_people_pizza

  # 답 반환하기
  return answer
```
