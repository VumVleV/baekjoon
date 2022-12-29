# 2588. 곱셈
```c++
#include <stdio.h>
int main(){
    int A, B, C, D, E, F;
    scanf("%d%d",&A,&B);
    C = A*(B%10);
    D = A*((B/10)%10);
    E = A*((B/100));
    F = 100*E+10*D+C;
    printf("%d\n%d\n%d\n%d",C,D,E,F);
}
```