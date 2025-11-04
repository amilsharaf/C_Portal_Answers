**Class Exercise 2**

**Problem Statement
Mr. Liam is an aspiring programmer exploring the use of logical operators. Create a simple program to assist Liam in understanding logical operations. 
Prompt two integers, a and b, and use logical operators to determine whether both values are non-zero. Display 'True' if both values are non-zero; otherwise, display 'False'.
Input format :
The input consists of two space-separated integers, representing a and b.
Output format :
The output displays "True" if both a and b are non-zero; otherwise, display "False".
**---

```c
// You are using GCC
#include<stdio.h>
int  main(){
    int a,b;
    scanf("%d %d",&a,&b);
    if ((a!=0)&&(b!=0)){
        printf("True");
    }else {
        printf("False");
    }
}
```
