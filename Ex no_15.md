# EX 15  C program  to check whether the given number is Armstrong number or not.
## DATE:
## AIM:
To write a C program  to check whether the given number is Armstrong number or not.

## Algorithm

1.Start the program and read the number n from the user.

2.Store the original value of n in a temporary variable N1.

3.Initialize sum = 0 and extract each digit using n % 10 inside a loop.

4.Add the cube of each digit to sum and update n = n / 10 until n becomes 0.

5.Compare sum with N1; if equal, print Armstrong number, otherwise print not an Armstrong number.

## Program:
```
#include<stdio.h>
int main()
{
    int r,n,sum=0,N1;
    scanf("%d",&n);
    N1=n;
    while(n>0)
    {
        r=n%10;
        sum=sum+r*r*r;
        n=n/10;
    }
    if(N1==sum)
    {
        printf("%d is armstrong number ",N1);
    }
    else
    {
        printf("%d is not a armstrong number",N1); 
    }
}
```

## Output:

<img width="645" height="176" alt="Screenshot 2026-03-19 140443" src="https://github.com/user-attachments/assets/52c07003-40e9-4488-90ba-dfb0d43f230a" />


## Result:
Thus the program was executed and the output was verified successfully.
