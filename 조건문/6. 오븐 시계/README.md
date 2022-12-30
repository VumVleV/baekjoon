# 2525. 오븐 시계
```c++
#include <stdio.h>
int main(){
    int A,B,C;
    scanf("%d%d%d",&A,&B,&C);
    if((((C%60)+B)<60)&&(((C/60)+A)<=23)){
        printf("%d %d",((C/60)+A),((C%60)+B));
    }
    else if((((C%60)+B)<60)&&(((C/60)+A)>23)){
        printf("%d %d",((C/60)+A)-24,((C%60)+B));
    }
    else if((((C%60)+B)>=60)&&(((C/60)+A+1)<=23)){
        printf("%d %d",((C/60)+A+1),((C%60)+B)-60);
    }
    else{
        printf("%d %d",((C/60)+A+1)-24,((C%60)+B)-60);
    }
    return 0;
}
```