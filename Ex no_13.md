# EX 13 To write a  C program to read the elements and print only the odd numbers in the n x n matrix
## DATE:
## AIM:
To write a  C program to read the elements and print only the odd numbers in the n x n matrix

## Algorithm

1.Start the program and read the size n of the matrix.

2.Declare a 2D array a[n][n] and read all the elements using nested loops.

3.Traverse the matrix again using nested loops.

4.For each element, check if it is odd using the condition a[i][j] % 2 != 0.

5.If the condition is true, print the position and value of the odd element, then stop the program.

## Program:
```
/*
Program to read the elements and print only the odd elements in the 2D array.
Developed by: 
RegisterNumber:  
#include<stdio.h>
int main()
{
    int i,j,n,a[10][10];
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {
        for(j=0;j<n;j++)
        {
            scanf("%d",&a[i][j]);
        }
    }
    for(i=0;i<n;i++)
    {
        for(j=0;j<n;j++)
        {
            if(a[i][j]%2!=0)
            {
                printf("a[%d][%d] is %d\n",i,j,a[i][j]);
            }
            
            
        }
        printf("\n");
    }
    
    
    
}
```

## Output:

<img width="609" height="436" alt="Screenshot 2026-03-19 135428" src="https://github.com/user-attachments/assets/620e013a-98a5-4f00-8748-8cf25434e41e" />


## Result:
Thus the program was executed and the output was verified successfully.
