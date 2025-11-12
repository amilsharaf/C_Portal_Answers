CE SESSION 1
-
_**Q1**_

__Problem Statement__

Rohan is developing a program for his college project that requires matrix multiplication. He needs to write a program that takes two 3×3 matrices, A and B, as input from the user and computes their product to generate matrix C. 
Help Rohan complete his program by implementing matrix multiplication and displaying the resulting matrix C.

**Input format :**
The input consists of the elements of array A in a 3x3 matrix, followed by a single line, followed by the elements of array B in a 3x3 matrix.

**Output format :**
The output displays the product of two matrices.

```c
#include<stdio.h>
#define n 3
int main() {
    int a[3][3], b[3][3], c[3][3], i, j, k;

    for (i = 0; i < n; i++) {
        for (j = 0; j < n; j++) {
            scanf("%d", & a[i][j]);
        }
    }

   
    for (i = 0; i < n; i++) {
        for (j = 0; j < n; j++) {
            scanf("%d", & b[i][j]);
        }
    }

    for (i = 0; i < n; i++) {
        for (j = 0; j < n; j++) {
            c[i][j] = 0;
            for (k = 0; k < n; k++) {
                c[i][j] += a[i][k] * b[k][j];
            }
        }
    }

    for (i = 0; i < n; i++) {
        for (j = 0; j < n; j++) {
            printf("%d ", c[i][j]);
        }
        printf("\n");
    }
    return 0;
}
```


_**Q2**_

__Problem Statement__
Aryan, a data analyst, is working on a project where he needs to analyze a 3×3 matrix. His task is to identify all odd numbers in the matrix, count them, and calculate their total sum. Additionally, he needs to display the array index positions of these odd elements.
Help Aryan write a program to store the matrix, find the sum of all odd elements, count them, and display their respective positions in the matrix.

**Input format :**
The input consists of the elements of a 3x3 matrix.

**Output format :**
The first output prints the odd elements and their array index positions.
The next output prints the total count of odd elements.
The last line of the output prints the sum of odd elements.
Refer to the sample output for the exact text and format.

**Code constraints :**
The given test cases fall under the following constraints:
The input must be a 3x3 matrix.

```c
#include <stdio.h>

int main() {
    int matrix[3][3];
    int sum = 0;
    int count = 0;
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            scanf("%d", &matrix[i][j]);
        }
    }

    printf("Odd elements and their positions:\n");
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            if (matrix[i][j] % 2 != 0) {  
                printf("Element %d at position [%d][%d]\n", matrix[i][j], i, j);
                sum += matrix[i][j];
                count++;
            }
        }
    }

    printf("Total count of odd elements: %d\n", count);
    printf("Sum of odd elements: %d", sum);

    return 0;
}
```

CE SESSION 2
-
