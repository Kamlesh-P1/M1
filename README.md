
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    char c1,c2,c3;
    scanf("%c %c %c",&c1,&c2,&c3);
    printf("%c %c %c",c3,c2,c1);
    return 0;
}
````
## OUTPUT:

<img width="1415" height="341" alt="image" src="https://github.com/user-attachments/assets/1f181f2f-3059-4277-b53e-982c24f21709" />
















## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
```
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    if(a>=0){
        printf("it's a positive number");
    }else{
        printf("it's not a positive number");
    }
    return 0;
}
```
# OUTPUT:
<img width="1472" height="452" alt="image" src="https://github.com/user-attachments/assets/8d14a868-f8fd-46f6-b3eb-1607cbff642e" />

<img width="1458" height="443" alt="image" src="https://github.com/user-attachments/assets/1344e186-2fc3-4399-a87b-7df20cc5fd37" />










# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
```
#include <stdio.h>
int main() {
    float n1,d1,n2,d2,r1,r2;
    printf("first Numerator and Denominator:");
    scanf("%f %f",&n1,&d1);
    printf("Enter second Numerator and Denominator:");
    scanf("%f %f",&n2,&d2);
    r1=n1/d1;
    r2=n2/d2;
    float main=(r1>r2)?r2:r1;
    printf("\nMinimum value after division is: %.2f",main);
    return 0;
}
```
## OUTPUT:

<img width="1409" height="484" alt="image" src="https://github.com/user-attachments/assets/1954bc96-e741-4add-bad7-3c66a636329b" />








## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
```
#include <stdio.h>
int main() {
    int n;
    printf("Enter a number:\n");
    scanf("%d",&n);
    if(n==1){
        printf("The entered value is equal to 1.");
    }else{
        printf("The entered value is not equal to 1.");
    }
    return 0;
}
```
## OUTPUT:

<img width="1432" height="459" alt="image" src="https://github.com/user-attachments/assets/b9b99e27-2609-43fa-9544-f12e96b4b954" />
<img width="1445" height="459" alt="image" src="https://github.com/user-attachments/assets/38e90899-cc49-44e3-b021-1e39bebfa6df" />








	

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:
```
#include <stdio.h>
int main() {
    int m1,m2,m3;
    float tot,per;
    printf("Enter marks for Three subjects:");
    scanf("%d %d %d",&m1,&m2,&m3);
    tot=m1+m2+m3;
    per=tot/3;
    printf("Total marks is: %.2f, and Percetnage is: %.2f\n",tot,per);
    if(m1>=40 && m2>=40 && m3>=40){
        if(per>=60){
            printf("Division = First");
        }
        else if(per>=48){
            printf("Division = Second");
        }
        else if(per>=36){
            printf("Division = Pass");
        }
        else{
            printf("Division = Fail");
        }
    }else{
        printf("Marks are not sufficient");
    }
    return 0;
}
```
## OUTPUT:
<img width="1459" height="795" alt="image" src="https://github.com/user-attachments/assets/f3cbcdd7-0159-4004-818a-2da1a8136dce" />

## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

