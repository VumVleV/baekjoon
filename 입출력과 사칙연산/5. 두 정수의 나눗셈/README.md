# 1000. A/B

(double)(a / b) 라고 적으면 원하는 값이 출력되지 않는다.   
이유는 a, b 모두 int형이기 때문에 정수 나누기로 계산한 뒤,   
 그 결과값만 실수형으로 변환하기 때문이다. (소수 아래 버림)   
(double)a / b 라고 적으면 a가 먼저 실수형이 되고,   
c언어 사칙연산 규칙에 의해 b도 실수형이 되어 소수 아래까지 계산된 결과까지 얻을 수 있다.

```c++
#include <stdio.h>
int main(){
    int A, B;
    scanf("%d%d",&A,&B);
    printf("%.9f\n",(double)A / B);
    return 0;
}
```