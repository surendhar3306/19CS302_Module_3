# EX 11 C program to convert a given value from binary to decimal using function with return type with out arguments
## DATE:
## AIM:
To write a C  program to convert a given value from binary to decimal using function with return type with out arguments

## Algorithm

1.Start the program and read the binary number from the user.

2.Call the function convert(n) to convert the binary number into decimal.

3.Inside the function, initialize variables sum = 0 and p = 0 (position).

4.Extract each digit of the binary number using modulus and multiply it with 
2p2, then add it to sum and increment p.

5.Return the calculated decimal value and display the result.

## Program:
```
#include<stdio.h>
#include<math.h>
int convert(int n)
{
    int r,sum=0,p=0;
    while(n>0)
    {
    r=n%10;
    sum=sum+r*pow(2,p);
    n=n/10;
    p++;
    }
    return sum;
}
int main()
{
    int n;
    scanf("%d",&n);
    int sum=convert(n);
    printf("%d in binary = %d in decimal",n,sum);
    return 0;
}
```

## Output:

<img width="596" height="169" alt="Screenshot 2026-03-19 134125" src="https://github.com/user-attachments/assets/de85df1e-1012-4fe2-bcdf-88348a18414e" />


## Result:
Thus the program was executed and the output was verified successfully.
