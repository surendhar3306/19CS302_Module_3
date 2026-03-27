# EX 14 C program to delete an element in array at specified position 

## DATE:
## AIM:
To write a C program  to delete an element in array at specified position.

## Algorithm

1.Start the program and read the number of elements n in the array.

2.Input the n elements into the array and display the original array.

3.Read the position pos of the element to be deleted.

4.Check if deletion is possible; if yes, shift elements from pos to n-1 one position to the left.

5.Decrease the array size by 1 and display the updated array after deletion.

## Program:
```
#include<stdio.h>
 
int main() 
{
    int array[100],i,n,pos;
 
    printf("Enter No.of.Elements to store in array:\n");    
    scanf("%d",&n);
  
    for (i=0;i<n;i++) 
    {
        scanf("%d",&array[i]);
    }
    printf("The original array elements are :\n");
    for(i=0;i<n;i++) 
    {
        printf("array[%d] = %d\n",i,array[i]);
    }

    printf("Enter the poisition to delete the element :\n");
    scanf("%d",&pos);
    if(n==pos)
    {
        printf("Deletion Not Possible");
    }
    else
    {
    for(i=pos;i<n-1;i++)
    {
        array[i]=array[i+1];
    }
    n=n-1;
    printf("The array elements after deletion :\n");
    for(i=0;i<n;i++) 
    {
        printf("array[%d] = %d\n",i,array[i]);
    }
    }
}
```

## Output:

<img width="619" height="834" alt="Screenshot 2026-03-19 140156" src="https://github.com/user-attachments/assets/ce92df7e-fcdd-4070-88ff-8ea81095fc1c" />


## Result:
Thus the program was executed and the output was verified successfully.
