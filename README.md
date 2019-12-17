____________________________________________________

   Name : Savi
   U Roll no : 1905395
   C Roll no : 1921094

____________________________________________________

1)To print College address.


#include<stdio.h>
int main()
{
    printf("Guru Nanak Dev Engineering College,\nGill Road,\nLudhiana, Punjab");
    return 0;
}
Program to add two integers.
#include<stdio.h>
int main()
{
    int a,b,sum;
    printf("Enter the value of first integer: ");
    scanf("%d", &a);
    printf("Enter the value of second integer: ");
    scanf("%d", &b);
    sum = a + b;
    printf("Sum is %d", sum);
    return 0;
}
____________________________________________________

2) Program to find quotient and remainder.

#include<stdio.h>
int main()
{
    int divisor, dividend, quotient, remainder;
    printf("Enter the value of divisor: ");
    scanf("%d", &divisor);
    printf("Enter the value of dividend: ");
    scanf("%d", &dividend);
    quotient = dividend/divisor;
    remainder = dividend%divisor; 
    printf("Qoutient is %d\n", quotient);
    printf("Remainder is %d", remainder);
    return 0;
} 
____________________________________________________

3) Program to swap two variables without 3rd variable.

#include<stdio.h>
int main()
{
    int a,b;
    printf("Enter the value of a = ");
    scanf("%d", &a);
    printf("Enter the value of b = ");
    scanf("%d", &b);
    a = a + b;
    b = a - b;
    a = a - b;
    printf("~~~~~~~~~~~~~~~~\nAfter Swap\n~~~~~~~~~~~~~~~~\n");
    printf("Value of a = %d\nValue of b = %d", a,b);
    return 0;
}

____________________________________________________
4) Program to check even odd number.

#include<stdio.h>
int main()
{
    int number;
    printf("Enter the number: ");
    scanf("%d", &number);
    if (number % 2 == 0)
    printf("Number is Even");
    else
    printf("Number is Odd");
    return 0;
}

____________________________________________________
5) Finding greteast of two numbers.

#include<stdio.h>
int main()
{
    int num1, num2;
    printf("Enter the first number: ");
    scanf("%d", &num1);
    printf("Enter the second number: ");
    scanf("%d", &num2);
    if (num1 > num2)
    printf("First Number is Greatest i.e %d", num1);
    else
    printf("Second Number is Greatest i.e %d", num2); 
    return 0;
}

____________________________________________________
6) Find greatest of three number .

#include<stdio.h>
int main()
{
    int a,b,c;
    printf("Enter the value of a ");
    scanf("%d", &a);
    printf("Enter the value of b ");
    scanf("%d", &b);
    printf("Enter the value of c ");
    scanf("%d", &c);
    if (a>b)
    {
        if(a > c)
        printf("a is the greatest");
        else
        printf("c is the greatest");
    }
    else
    {
        if (b > c)
        printf("b is the greatest");
        else
        printf("c is the greatest");
        
    }
    return 0;
    
}

____________________________________________________
7) Program to assign grade to student according to percentage.

#include<stdio.h>
int main()
{
    int marks;
    printf("~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\nSchema for marks and grades\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\nMarks\tGrade\n0-30\tF\n31-50\tD\n51-70\tC\n71-80\tB\n81-90\tA2\n91-100\tA1\n");
    printf("Enter is the marks (Out of 100): ");
    scanf("%d", &marks);
    if (marks>=0)
    {
        if (marks <= 90)
            {
                if (marks <= 80)
                {
                    if (marks <= 70)
                    {
                        if (marks <= 50)
                        {
                            if (marks <= 30)
                            printf("Grade is F");
                            else
                            printf("Grade is D");
                        }
                        else
                        printf("Grade is C");
                    }
                    else
                    printf("Grade is B");
                }
                else
                printf("Grade is A2");
            }
        else
        printf("Grade is A1");
    }
    else 
    printf("Invalid Input");
    return 0;
}
____________________________________________________

8) Program to print roots of quadratic equation.

#include<stdio.h>
#include<math.h>
int main()
{
    int a,b,c,root1,root2;
    printf("~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\nSchema of a Quadratic Equation is a(x^2) + b(x) + c = 0\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n");
    printf("Enter is value of a ");
    scanf("%d", &a);
    printf("Enter is value of b ");
    scanf("%d", &b);
    printf("Enter is value of c ");
    scanf("%d", &c);
    root1 = ((-b) + sqrt((b*b) - (4*a*c)))/(2*a);
    root2 = ((-b) - sqrt((b*b) - (4*a*c)))/(2*a);
    printf("Roots are %d and %d", root1,root2);
    return 0;
}
____________________________________________________

9) Program to check year is leap or not.

#include<stdio.h>
int main()
{
    int year;
    printf("Enter the year: ");
    scanf("%d", &year);
    if (year%4 == 0)
    printf("%d is a Leap Year", year);
    else 
    printf("%d is not a Leap Year", year);
    return 0;
}

____________________________________________________
10) Program to print table of 5.


#include<stdio.h>
int main()
{
    int num,x;
    printf("Enter the number of mutiples of 5 you want: ");
    scanf("%d", &num);
    for (x=1; x<=num; x++)
    {
        printf("5\t*\t%d\t=\t%d\n", x,x*5);
    }
    return 0;
}

____________________________________________________
11) To make simple calculator using switch case.

#include<stdio.h>
int main()
{
    double num1,num2;
    char operator;
    printf("Select the Operator (+ - * /)");
    scanf("%c", &operator);
    printf("\nEnter the numbers: ");
    scanf("%lf %lf", &num1,&num2);
    switch(operator)
    {
        case '+':
        printf("%.2lf + %.2lf = %.2lf", num1,num2,num1+num2);
        break;
        case '-':
        printf("%.2lf - %.2lf = %.2lf", num1,num2,num1-num2);
        break;
        case '*':
        printf("%.2lf * %.2lf = %.2lf", num1,num2,num1*num2);
        break;
        case '/':
        printf("%.2lf / %.2lf = %.2lf", num1,num2,num1/num2);
        break;
        default:
        printf("Invalid Operator");
    }

    return 0;
}

____________________________________________________
12) To calculate reverse of a number.

#include<stdio.h>
int main()
{
    int num, reverse=0;
    printf("Enter the number: ");
    scanf("%d", &num);
    while(num != 0)
    {
        reverse = reverse * 10;
        reverse = reverse + num%10;
        num = num/10;
    }
    printf("Reverse of the Entered Number is %d", reverse);
    return 0;
}

____________________________________________________
13) To check whether number is palindrome or not.

 #include<stdio.h>
int main()
{
    int num,original, reverse=0;
    printf("Enter the number: ");
    scanf("%d", &num);
    original = num;
    while(num != 0)
    {
        reverse = reverse * 10;
        reverse = reverse + num%10;
        num = num/10;
    }
    if (original == reverse)
    printf("Number is a palindrome");
    else 
    printf("Number is not a palindorme");
    return 0;
}

____________________________________________________
14) To check whether a number is prime or not.

#include<stdio.h>
int main()
{
    int num, k=0, x;
    printf("Enter the number: ");
    scanf("%d", &num);
    for (x=1; x<=num; x++)
    {
        if (num%x == 0)
        {
            k++;
        }
    }
    if (k == 2)
    printf("Number is a Prime Number");
    else 
    {
        if (k == 1)
        printf("Number is neither a prime nor a composite");
        else
        printf("Number is not a prime number");
    }
}
____________________________________________________

15) Program to print prime numbers from 1 to 100.
#include <stdio.h>
 
int main()
{
  int i, Number, count; 
  
  printf(" Prime Number from 1 to 100 are: \n"); 
  for(Number = 1; Number <= 100; Number++)
  {
    count = 0;
    for (i = 2; i <= Number/2; i++)
    {
  	if(Number%i == 0)
  	{
     	  count++;
  	  break;
	}
    }
    if(count == 0 && Number != 1 )
    {
	printf(" %d ", Number);
    }  
  }
  return 0;
} 

____________________________________________________
16) Program to check whether a number is armstrong or not.

#include<stdio.h>
int main()
{
    int number,remainder,sum=0,original_number;
    printf("Enter the Number: ");
    scanf("%d", &number);
    original_number = number;
    while(number>0)
    {
        remainder = number%10;
        sum = sum+(remainder*remainder*remainder);
        number = number/10;
    }
    if (original_number == sum)
    printf("Number is a Armstrong Number");
    else 
    printf("Number is not a Amrstrong Number");
    return 0;
}

____________________________________________________
17) Print the following patterns:

i) Pattern 1.
#include<stdio.h>
int main()
{
    int x,y;
    for(x=1; x<5; x++)
    {
        for (y=1; y<=x; y++)
        {
            printf("%d", y);
        }
        printf("\n");
    }
    return 0;} 


ii) Pattern 2.

#include<stdio.h>
int main()
{
    int x,y,z=1;
    for (x=1; x<5; x++)
    {
        for (y=1; y<=x; y++)
        {
            printf("%d", z++);
        }
        printf("\n");
    }
    return 0;
}


iii) Pattern 3.
#include<stdio.h>
int main()
{
    int p,q,r,s,t;
    for (p=1; p<5; p++)
    {
        for (q=1; q<5-p; q++)
        {
            printf(" ");
        }
        for (r=1; r<=p; r++)
        {
            printf("%d", r);
        }
        for (s=p-1; s>=1; s--)
        {
            printf("%d", s);
        }
        printf("\n");
    }
    return 0;
}

____________________________________________________
18) Program to find largest from 1 dimensional array.

#include<stdio.h>
int main()
{
    int i, n, arr[5],largest;
    for(i = 0; i < 6; i++)
    {
       printf("Enter Number %d: ", i);
       scanf("%d", &arr[i]);
    }
    for(i = 0; i < 6; i++)
    {
       if(largest < arr[i])
           largest = arr[i];
    }
    printf("Largest element = %d", largest);
    return 0;
}

____________________________________________________
19) To find sumof the N natural numbers in an array.

#include<stdio.h>
int main()
{
    int arr[1000],n,x,y,sum=0;
    printf("Enter the number of elements you want to input(From 1 to 1000): ");
    scanf("%d", &n);
    for (x=0; x<n; x++)
    {
        printf("Enter Element %d: ", x+1);
        scanf("%d", &arr[x]);
    }
    for (y=0; y<n; y++)
    {
        sum += arr[y];
    }
    printf("Sum of above array elements is %d", sum);                    
    return 0;
}

____________________________________________________

20) Program to add two matrices .

#include<stdio.h>
int main() 
{ 
    int A[4][4] = { {1, 1, 1, 1},{2, 2, 2, 2},{3, 3, 3, 3}, {4, 4, 4, 4}}; 
  
    int B[4][4] = { {1, 1, 1, 1}, {2, 2, 2, 2},{3, 3, 3, 3},{4, 4, 4, 4}}; 
  
    int C[4][4];
    int i, j; 
    int k, l; 
    for (k = 0; k < 4; k++)
    {
      for (l = 0; l < 4; l++) 
      {
          C[k][l] = A[k][l] + B[k][l];   
      }        
    } 
    printf("Result matrix is \n"); 
    for (i = 0; i < 4; i++) 
    { 
        for (j = 0; j < 4; j++)
        {
            printf("%d ", C[i][j]);
        }    
        printf("\n"); 
    } 
  
    return 0; 
}

________×_____________________×________________×_______
