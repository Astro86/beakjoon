# 백준 2455 - 지능형 기차

![](2455.jpeg)

## 채점 현황
![](2455_score.png)

## 전체 소스 코드
```cpp
#include <iostream>
using namespace std;

int in[4];
int off[4];
int num;
int maxNum;

int main(void) {
    for (int i = 0; i < 4; i++) {
        cin >> off[i] >> in[i];
    }

    for (int i = 0; i < 4; i++) {
        num = num - off[i];
        num = num + in[i];

        if (maxNum < num) {
            maxNum = num;
        }
    }

    cout << maxNum << '\n';
    return 0;
}
```