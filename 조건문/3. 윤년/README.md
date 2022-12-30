# 2753. 윤년
```c++
#include <stdio.h>
int main(){
    int A;
    scanf("%d",&A);
    if(A%400==0){
        printf("%d",1);
    }
    else if(A%100==0){
        printf("%d",0);
    }
    else if(A%4==00){
        printf("%d",1);
    }
    else{
        printf("%d",0);
    }
    return 0;
}
```