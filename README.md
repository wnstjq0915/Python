# Python

## 함수
### 예시1
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

### 예시2
- 예시1은 3명으로 정해져 있는데  
예시2는 k명으로 주기
```python
def pizza_mukbang(n, k):

  remain_pizza = n

  # 세 명이서 먹을 수 있는 피자조각
  three_people_pizza = k * 5

  # 답 계산
  answer = n - three_people_pizza

  # 답 반환하기
  return answer
```

### 예시3
- 예시1 답에서 if문을 활용하여 사람이 먹을 때마다 print하기
```python
def pizza_mukbang(remain_pizza):
  # remain_pizza는 남은 피자수

  # 한명 먹방
  if remain_pizza - 5 > 0:
    remain_pizza = remain_pizza - 5
    print('한명이 먹었습니다!')
  else:
    print('한명이 먹었을 때 남는 피자가 없습니다.')
    return 0

  # 두명 먹방
  if remain_pizza - 5 > 0:
    remain_pizza = remain_pizza - 5
    print('두명이 먹었습니다!')
  else:
    print('두명이 먹었을 때 남는 피자가 없습니다.')
    return 0

  # 세명 먹방
  if remain_pizza - 5 > 0:
    remain_pizza = remain_pizza - 5
    print('세명이 먹었습니다!')
    return remain_pizza
  else:
    print('세명이 먹었을 때 남는 피자가 없습니다.')
    return 0
```
- 추가로 남는 피자가 없을 경우 몇 조각의 피자가 부족한지도 같이 print해보기
