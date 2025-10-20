# NAME: Ritika. S
# REGISTER NO: 25009202

# EXP NO: 3a) C PROGRAM TO PREPARE EMI CALCULATION FOR 251000,8.5,5 YEARS USING FUNCTION WITH RETRUN TYPE WITH ARGUMENTS.

# AIM: 
To write a program to prepare EMI calculation for 251000,8.5,5years using function with return type with arguments.

# ALGORITHM:
1. Declare a float function and the values inside the function.
2. Write all the formulae inside the calculate the EMI value.
3. In main() function, call the EMI function.
4. Print the EMI value using printf function.


# PROGRAM:
```
#include <stdio.h>
#include<math.h>
float calculateEMI()
{
    float principal=251000,rate=8.5,tenure=5;
    rate=rate/(12*100);
    tenure=tenure*12;
    float emi=(principal*rate*pow(1+rate,tenure))/(pow(1+rate,tenure)-1);
    return emi;
}
int main()
{
    float emi=calculateEMI();
    printf("Monthly EMI is= %.3f",emi);
    return 0;
}
```

# OUTPUT:
![alt text](<Screenshot 2025-10-20 130632.png>)

# RESULT:
Thus, the program is verified successfully.


# EXP NO: 3b) C PROGRAM TO CHECK WHETHER THE GIVEN NUMBER IS PRIME OR NOT.

# AIM: 
To write a C program  to check whether the given number is prime or not.

# ALGORITHM:
1. Take the number from the user as input using scanf function.
2. Using for loop, start the iteration.
3. Using if condition, check if the number is a prime or not.
4. If the condition is not true, then the else block will be executed.
5. Print the statement using printf function. 


# PROGRAM:
```
#include<stdio.h>
#include<math.h>
int main()
{
  int num;
  scanf("%d",&num);
  for(int div=2;div<num;div++)
  {
    if((num%div)==0)
    {
      printf("%d is not a prime number.",num);
      return 0;
    }
    else printf("%d is a prime number.",num);
    return 0;
  }
}
```

# OUTPUT:
![alt text](<Screenshot 2025-10-20 131940.png>)

# RESULT:
Thus, the program is verified successfully.



# EXP NO: 3c) C PROGRAM TO READ N ELEMENTS AS INPUT AND PRINT THE SECOND ELEMENT OF THE ARRAY(INTEGER).

# AIM: 
To write a C program to read n elements as input and print the second element of the array (integer).

# ALGORITHM:
1. Take the number from the user as input using scanf function.
2. Declare an integer array of size n.
3. Using for loop, take the array from the user as input.
4. Print the second element of the array using it's index value. 

# PROGRAM:
```
#include<stdio.h>
int main()
{
  int n,ind;
  scanf("%d",&n);
  int arr[n];
  for(ind=0;ind<n;ind++)
  {
    scanf("%d ",&arr[ind]);
  }
  printf("%d",arr[1]);
return 0;
}
```

# OUTPUT:
![alt text](<Screenshot 2025-10-20 132521.png>)

# RESULT:
Thus, the program is verified successfully.


# EXP NO: 3d) C PROGRAM TO FIND THE SMALLEST ELEMENT IN THE GIVEN ARRAY:
int arr[]={12,1234,45,67,1}

# AIM: 
To write a C program to find the smallest element in the given array:

int arr[] = { 12, 1234, 45, 67, 1 }

# ALGORITHM:
1. Declare the given integer array inside main() function.
2. Declare the first array element as the samllest. 
3. Using for loop, take the array from the user as input.
4. Using if condition, check whether the current array element is less than the smallest.
5. If the condition is true, then the cuurent array element will be the smallest element.
6. Print the smallest element in the given array using printf function.

# PROGRAM:
```
#include<stdio.h>
int main()
{
    int arr[]={12,1234,45,67,1};
    int smallest=arr[0];
    for(int ind=1;ind<5;ind++)
    {
        if(arr[ind]<smallest)
        {
            smallest=arr[ind];
        }
    }
    printf("%d",smallest);
    return 0;
}
```

# OUTPUT:
![alt text](<Screenshot 2025-10-20 133350.png>)

# RESULT:
Thus, the program is verified successfully.


# EXP NO: 3e) C PROGRAM TO PRINT THE FOLLOWING PATTERN

5 5 5 5 5 5 5 5 5 

5 4 4 4 4 4 4 4 5 

5 4 3 3 3 3 3 4 5 

5 4 3 2 2 2 3 4 5 

5 4 3 2 1 2 3 4 5 

5 4 3 2 2 2 3 4 5 

5 4 3 3 3 3 3 4 5 

5 4 4 4 4 4 4 4 5 

5 5 5 5 5 5 5 5 5 

# AIM: 
To write a C program to print the following pattern.

5 5 5 5 5 5 5 5 5 

5 4 4 4 4 4 4 4 5 

5 4 3 3 3 3 3 4 5 

5 4 3 2 2 2 3 4 5 

5 4 3 2 1 2 3 4 5 

5 4 3 2 2 2 3 4 5 

5 4 3 3 3 3 3 4 5 

5 4 4 4 4 4 4 4 5 

5 5 5 5 5 5 5 5 5 

# ALGORITHM:
1. Declare the function to find the minimum of values.
2. In main() function, declare the row, col, val,size and the N value.
3. Using for loops, write the calculation for the value.
4. Print the result and for each result print a new line.

# PROGRAM:
```
#include<stdio.h>
#define min(a,b)(a)<(b)?(a):(b)
int main()
{
    int N,row,col,val,size;
    N=5;
    size=N*2-1;
    for(row=1;row<=size;row++)
    {
        for(col=1;col<=size;col++)
        {
            val=min(min(row,col),min(size-row+1,size-col+1));
            printf("%d ",N-val+1);
        }
        printf("\n");
    }
    return 0;
}
```

# OUTPUT:
![alt text](<Screenshot 2025-10-20 134247.png>)

# RESULT:
Thus, the program is verified successfully.