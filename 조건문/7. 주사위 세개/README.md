# 2480. 주사위 세개
```c++
#include <stdio.h>
int main(){
    int A,B,C;
    scanf("%d%d%d",&A,&B,&C);
    if((A==B)&&(B==C)){
        printf("%d",10000+1000*A);
    }
    else if(A==B){
        printf("%d",1000+100*A);
    }
    else if(B==C){
        printf("%d",1000+100*B);
    }
    else if(A==C){
        printf("%d",1000+100*C);
    }
    else if((A>B)&&(A>C)){
        printf("%d",100*A);
    }
    else if((B>C)&&(B>A)){
        printf("%d",100*B);
    }
    else{
        printf("%d",100*C);
    }
    return 0;
}
```
```c++
#include <stdio.h>
int max(int a, int b, int c){
    if(a>=b&&a>=c){
        return a;
    } else if(b>=a&&b>=c){
        return b;
    } else{
        return c;
    }
    }
int main(){
    int A,B,C,V;
    scanf("%d%d%d",&A,&B,&C);
    if(A==B&&B==C){
        V = 10000+1000*A;
    } else if(A==B){
        V = 1000+A*100;
    } else if(B==C){
        V = 1000+B*100;
    } else if(A==C){
        V = 1000+A*100;
    } else{
        V = max(A,B,C)*100;
    }
    printf("%d",V);
    return 0;
    }
```