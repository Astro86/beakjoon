# 백준 10995 - 별 찍기 - 20

## 문제
예제를 보고 규칙을 유추한 뒤에 별을 찍어 보세요.


## 입력
첫째 줄에 N(1 ≤ N ≤ 100)이 주어진다.

## 출력
첫째 줄부터 차례대로 별을 출력한다.

## 파이썬 코드
```python
n = int(input())
for i in range(1, n+1):
    if(i % 2 == 0):
        print(' ', end='')
    print('* '*n)
```
