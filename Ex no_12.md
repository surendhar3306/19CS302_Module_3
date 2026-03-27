# EX 12 C program  to check whether 87 is prime or not
## DATE:
## AIM:
To write a C program  to check whether 87 is prime or not

## Algorithm

1.Start the program and initialize the number n = 87 and set flag = 0.

2.Use a loop from i = 2 to n/2 to check for factors.

3.Inside the loop, check if n % i == 0; if true, set flag = 1 and break the loop.

4.After the loop, check if flag == 0; if true, the number is prime, otherwise not prime.

5.Display the result and stop the program.

## Program:
```
#include <stdio.h>
int main() {
  int n=87, i, flag = 0;
 
  for (i = 2; i <= n / 2; ++i) {
    
    if (n % i == 0) {
      flag = 1;
      break;
    }
  }

  if (n == 1) {
    printf("1 is neither prime nor composite.");
  } 
  else {
    if (flag == 0){
      printf("%d is a prime number.", n);
    }
    else{
      printf("%d is not a prime number.", n);
    }
  }

  return 0;
}
```

## Output:

<img width="604" height="125" alt="Screenshot 2026-03-19 134746" src="https://github.com/user-attachments/assets/543d42e8-dfe3-4393-8ed6-be9fae15a97c" />


## Result:
Thus the program was executed and the output was verified successfully.
