# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int m,n;
    scanf("%d %d",&m,&n);
    if (m % 2 != 0) 
    {
        m++;
    }
    for (int i = m; i <= n; i += 2)
    {
        printf("%d ", i);
    }

 
    return 0;
}
```

## OUTPUT:

![Screenshot (250)](https://github.com/user-attachments/assets/cfd4ff2b-be4e-46ef-9d24-0c83b2eeb364)









## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include <stdio.h>

int main() {
    int n;
    scanf("%d", &n);
for (int i = 0; i < n; i++) {
        for (int j = 0; j < n - i - 1; j++) {
            printf(" ");
        }
        for (int j = 0; j < 2 * i + 1; j++) {
            printf("A");
        }
        printf("\n");
    }
    return 0;
}

```

## OUTPUT:
![Screenshot (252)](https://github.com/user-attachments/assets/e2619ab7-17cc-4244-8269-25f2f52aaf9b)





## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
#include<stdio.h>
void add(int a,int b);
void subtract(int a,int b);
int main()
{
    int a,b;
    scanf("%d%d",&a,&b);
    add(a,b);
    subtract(a,b);
    return 0;
}
   void add(int a,int b)
   {
       printf("Addition: %d\n",a+b);
   }
   void subtract(int a,int b) 
   {
       printf("Subtraction: %d\n",a-b);
   }
```


## OUTPUT:

![Screenshot (254)](https://github.com/user-attachments/assets/30bff497-fe43-455e-92de-475ee6b0639b)





## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int m,n;
    scanf("%d%d",&m,&n);
    for(int i=1;i<=m;i++)
    {
        for(int j=1;j<=n;j++)
        {
            if(i%2==1)
               printf("0");
            else
              printf("1");
        }
        printf("\n");
    }
    return 0;
}
```

## OUTPUT:

![Screenshot (256)](https://github.com/user-attachments/assets/e4457baf-52aa-4108-8d0d-c9f2eb0deb40)



## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include<stdio.h>
int fact(int);
int main()
{    
    int n;
    scanf("%d",&n);
    fact(n);
    return 0;
}
int fact(int n)
{
    int i,fact=1;
    
    for(i=1; i<n; i++)
    {
        fact=fact*i;
        
    }
    printf("Factorial value is: %d",fact); 
        return fact;
}
```

## OUTPUT:
![Screenshot (259)](https://github.com/user-attachments/assets/908eb4d2-e708-4119-8826-224f0d46398c)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
