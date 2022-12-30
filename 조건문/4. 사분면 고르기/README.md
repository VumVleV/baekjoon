# 14681, 사분면 고르기
```c++
#include <stdio.h>
int main(){
    int A,B;
    scanf("%d%d",&A,&B);
    if(A>0&&B>0){
        printf("%d",1);
    }
    else if(A>0){
        printf("%d",4);
    }
    else if(B>0){
        printf("%d",2);
    }
    else{
        printf("%d",3);
    }
    return 0;
}
```