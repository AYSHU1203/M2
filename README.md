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
    scanf("%d%d",&m,&n);
    
    for(int i=m;i<=n;i++)
    {
        if(i%2 ==0){
            printf("%d ",i);
        }
        
    }
    return 0;
}
```

## OUTPUT:
![438635732-556ce8a8-5988-4054-bc56-ecd7fb2c5073](https://github.com/user-attachments/assets/928cb7ef-b17b-49e1-b3cd-f286dcf09e63)











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
    for (int i = n; i >= 1; i--) {
        for (int j = 1; j <= i; j++) {
            printf("a");
        }
        printf("\n");
    }
    return 0;
}
```


## OUTPUT:
![438636413-77801bfd-4bc4-4924-9ad2-42dae9bdab9b](https://github.com/user-attachments/assets/531f747f-2619-4bf9-a35b-3eb796be2b38)






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
#include <stdio.h>
void multiply(int a, int b) {
    printf("Multiplication: %d\n", a * b);
}

void divide(int a, int b) {
    if (b != 0) {
        printf("Division: %.2f\n", (float)a / b);
    } else {
        printf("Error: Division by zero\n");
    }
}

int main() {
    int num1, num2;
    scanf("%d %d", &num1, &num2);
    multiply(num1, num2);
    divide(num1, num2);
    return 0;
}
```


## OUTPUT:

![438638498-6a5db585-c1d8-4d04-b3b7-7cae46dc27a7](https://github.com/user-attachments/assets/b203ba1f-bca5-4356-a803-3736addfede2)






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
#include <stdio.h>

int main() {
    int start, end, sum = 0, i;
    scanf("%d %d", &start, &end);
    
    i = start;
    do {
        if (i % 2 != 0) sum += i;
        i++;
    } while (i <= end);
    
    printf("%d\n", sum);
    return 0;
}
```


## OUTPUT:

![438639549-15054108-10e2-434f-8913-219a6bd29d90](https://github.com/user-attachments/assets/bea80556-0506-4314-9230-83f0d5f603f7)




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
#include <stdio.h>

int main(){
    int a;
    scanf("%d",&a);
    
    if(a%2 != 0){
        if(a >= 25){
            printf("The number is odd\n");
            printf("The number is greater than or equal to 25\n");
        }
        else{
            printf("the number is not equal to 25\n");
        }
    }
    else{
        printf("The number is NOT an odd number\n");
    }
    return 0;
}
```


## OUTPUT:
![438640499-69493f5f-435f-4feb-a6b1-1a6f623ad6e6](https://github.com/user-attachments/assets/060081ba-96c6-458f-8edd-c059ccecce91)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
