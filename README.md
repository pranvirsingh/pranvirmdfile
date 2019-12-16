#PPS                    
                    Programming for Problem Solving

**1) Program to Print Welcome Message**
```C
#include <stdio.h>

void main() {
puts("Budding Engineers ! Welcome to Guru Nanak Dev Engeering College");
}
```

OUTPUT:

> Budding Engineers ! Welcome to Guru Nanak Dev Engeering College
> 



**2) Program to print your address using puts**

```C
#include <stdio.h>

void main()
{
puts("Pranvir Singh");
puts("House no. 107");
puts("Guru Nanak Nagar Block-B");
puts("Gill")
puts("Distt. Ludhiana");
puts("141116");
}
```

**OUTPUT:**

> Pranvir Singh
> House no. 107
> Guru Nanak Nagar Ludhiana
> Gill
> distt. Ludhiana
> 141116

**3) Program to find sum 0f two number:**

```#include <stdio.h>
int num1, num2;

void main(){
printf("Welcome to the program to add to nunber\n");
printf("Write the numbers to be added:\n");
scanf("%d %d", &num1 ,&num2);
printf("The sum of two number is:");
printf("%d",num1 + num2);
}
```

**OUTPUT:**

> Welcome to the program to add to nunber
> Write the numbers to be added:
> 34
> 67
> The sum of two number is:101


**4)Program to convert temperature degree celcius to degree Farenheit**

```include<stdio.h>
float temp_in_c, temp_in_f;
int main(){
printf("Welcome to the temperature converter\n");
printf("Please Enter the temperature in degree celcius:\n");
scanf("%f",&temp_in_c);
temp_in_f = (temp_in_c * 9)/5  + 32;
printf("%f",temp_in_f);
}
```

OUTPUT:

> Welcome to the temperature converter
> Please Enter the temperature in degree celcius:
> 34
> 93.199997

**5)Program to find area and perimeter of circle**
```C
#include <stdio.h>
 
#define PI 3.14f
 
int main()
{
    float rad,area, perm;
 
    printf("Enter radius of circle: ");
    scanf("%f",&rad);
 
    area=PI*rad*rad;
    perm=2*PI*rad;
 
    printf("Area of circle: %f \nPerimeter of circle: %f\n",area,perm);
    return 0;
}
```
**OUTPUT:**
>Enter radius of circle: 2.34
>Area of circle: 17.193384
>Perimeter of circle: 14.695200

**6) Program to find factorial of a number**

```#include <stdio.h>
int d;
int num = 1;
int main(){
printf("Enter the number whose factorial to be found:\n");
scanf(" %d",&d);
for(d; d>0; d--){
num = num *d ;
}
printf(" The factorial is %d",num);
return 0;

}
```

**OUTPUT:**

> Enter the number whose factorial to be found:
> 9
> The factorial is 362880

**7)Program to swap a number without using two numbers:**
```#include <stdio.h>
 
int main()
{
   int a, b;
   
   printf("Input two integers (a & b) to swap\n");
   scanf("%d%d", &a, &b);
   
   a = a + b;
   b = a - b;
   a = a - b;
 
   printf("a = %d\nb = %d\n",a,b);
   return 0;
}
```

**OUTPUT:**
> Input two integers (a & b) to swap
> 3
> 7
> a = 7
> b = 3


**8)Program to check if the Number is odd or even:**

```#include <stdio.h>
int num;
int main(){
printf("Please enter the number to check if it's even or odd");
scanf("%d",&num);
if (num%2 == 0)
printf("The number is Even:\n");
else
printf("The number id Odd");
}
```

**OUTPUT:**

> Please enter the number to check if it's even or odd:
> 54
> The number is Even

**9)Program to reverse a number**

```#include <stdio.h>
int x,num, rev = 0;
int main()
{    printf("Enter the number to be reversed: \n");
    scanf("%d", &num);
    while(num > 1){
        x = num % 10;
        rev = rev * 10 + x;
        num = num / 10;
    }
    printf("The reversed number is : %d \n", rev);
    return 0;
}
```

OUTPUT:
> Enter the number to be reversed: 
> 789342
> The reversed number is 243987

**10)Program of FizzBuzz:**

```#include<stdio.h>
int num;
int main(){
printf("Welcome to the Fizz Buzz Program");
printf("Enter The number");
scanf("%d",&num);
if (num%3 == 0 && num%5 !=0)
printf("Fizz");
if (num%3 != 0 && num%5 == 0)
printf("Buzz");
if (num%3 == 0 && num%5 == 0)
printf("FizzBuzz"); 
}
```

**OUTPUT:**
> Welcome to the Fizz Buzz Program
> Enter The number:45
> FizzBuzz

**11)Program to show days of week using Switch Case:**
```C

#include <stdio.h>

int main()
{
    int week;
    
    /* Input week number from user */
    printf("Enter week number(1-7): ");
    scanf("%d", &week);
    
    switch(week)
    {
        case 1: 
            printf("Monday");
            break;
        case 2: 
            printf("Tuesday");
            break;
        case 3: 
            printf("Wednesday");
            break;
        case 4: 
            printf("Thursday");
            break;
        case 5: 
            printf("Friday");
            break;
        case 6: 
            printf("Saturday");
            break;
        case 7: 
            printf("Sunday");
            break;
        default: 
            printf("Invalid input! Please enter week number between 1-7.");
    }

    return 0;
}
```
**OUTPUT:**
>Enter week number(1-7): 1
>Monday

**12) Program of calculator using Switch Case:**

```include <stdio.h>

void main()
{
        int num1, num2, res;
        char op;
        printf("Enter the First number");
        scanf("%d", &num1);
        printf("Enter the second number");
        scanf("%d", &num2);
        printf("What operation do you want to perform /
        /s for sum, b for subtract, d for divide , m for multiply ");
        scanf(" %c",&op);

switch(op)
{
        case 's':
                res = num1 + num2;
                printf("The sum of the chosen number is %d", res );
        break;

        case 'b':
                res = num1 - num2;
                printf("The difference of the chosen number is %d", res );
        break;  

        case 'd':
                res = num1 / num2;
                printf("The ratio of the chosen number is %d", res );
        break;

        case 'm':
                res = num1 * num2;
                printf("The product of the chosen number is %d\n", res );
        break;

        default:
                printf("Get your eyes checked by Doctor ");     
        break;
        }

}
```

**OUTPUT:**

> Enter the First number:23
> Enter the second number:45
> What operation do you want to perform s for sum, b for subtract, d for divide , m for multiply m
> The product of the chosen number is :1035

**13) Program to check a Leap year**

```#include<stdio.h>
int year;
int main(){
printf("Hi welcome to the program that checks the leap year");
printf("Please enter the value of the year\n");
scanf("%d",&year);
if (year%4 == 0)
printf("The year is a leap year");
else
printf("The year is not a leap year");

}
```
**OUTPUT:**

> Hi welcome to the program that checks the leap yearPlease enter the value of the year
> 2005
> The year is not a leap year


**14) Program to Check if a number is Prime**

```#include<stdio.h>
void main()
{
int num,sum=0;
printf("enter the number which you want check to wheather prime or not\n");
scanf("%d",&num);
if(num==1)
printf("number is neither prime nor composite\n");
else if(num<1)
printf("enter number greater than 1\n");
else
{
for(int i=2;i<n;i++)
{
if(n%i==0)
sum++;
}
if(sum==0)
printf("The number is prime\n");
else 
printf("The number is composite\n");
}
}
```

**OUTPUT:**
> enter the number which you want check to wheather prime or not
> 71
> The number is prime

**15)Program to check if a number is Palindrome**

```#include<stdio.h>

int x,num, num_loop,rev= 0;
int main(){
printf("Welcome to the palindrome function\n");
printf("Enter the number:\n");
scanf("%d",&num);
num_loop = num;
while(num_loop > 1){
x = num_loop % 10;
rev = rev * 10 +x;
num_loop = num_loop/10;
}
if (rev == num)
printf("oh yes ! You wrote a palindrome number");
else
printf("sorry the number is not a palindrome");
}
```
**OUTPUT:**
> Welcome to the palindrome function
> Enter the number:
> 234565432
> oh yes ! You wrote a palindrome number

**16)Program to check a palindrome of Word**
   ```C
 
#include <stdio.h> 
#include <string.h> 
  
// A function to check if a string str is palindrome 
void isPalindrome(char str[]) 
{ 
    // Start from leftmost and rightmost corners of str 
    int l = 0; 
    int h = strlen(str) - 1; 
  
    // Keep comparing characters while they are same 
    while (h > l) 
    { 
        if (str[l++] != str[h--]) 
        { 
            printf("%s is Not Palindrome", str); 
            return; 
        } 
    } 
    printf("%s is palindrome", str); 
} 
  
// Driver program to test above function 
int main() 
{ 
    isPalindrome("abba"); 
    isPalindrome("abbccbba"); 
    isPalindrome("geeks"); 
    return 0; 
}

```
**OUTPUT:**
>abba is palindrome
>abbccbba is palindrome
>geeks is Not Palindrome




**17)Program to print fibonacci series**

```#include<stdio.h>
int a,b,c,i;
int main(){

printf("Enter the first number of the series");
scanf("%d",&a);
printf("Enter the second number");
scanf("%d",&b);
for(i=0;i<20;i++){
c = a+b;
printf("%d\n",c);
a = b;
b = c;
}
}
```
**OUTPUT:**

> Enter the first number of the series5
> Enter the second number6
> 11
> 17
> 28
> 45
> 73
> 118
> 191
> 309
> 500
> 809
> 1309
> 2118
> 3427
> 5545
> 8972
> 14517
> 23489
> 38006
> 61495
> 99501


**18)Program to Enter and Display Elements of 1D Array:**
```C
    #include <stdio.h>
     
    int main()
    {
       int array[100], position, c, n, value;
     
       printf("Enter number of elements in array\n");
       scanf("%d", &n);
     
       printf("Enter %d elements\n", n);
     
       for (c = 0; c < n; c++)
          scanf("%d", &array[c]);
     
       printf("Enter the location where you wish to insert an element\n");
       scanf("%d", &position);
     
       printf("Enter the value to insert\n");
       scanf("%d", &value);
     
       for (c = n - 1; c >= position - 1; c--)
          array[c+1] = array[c];
     
       array[position-1] = value;
     
       printf("Resultant array is\n");
     
       for (c = 0; c <= n; c++)
          printf("%d\n", array[c]);
     
       return 0;
    }
    
```
**OUTPUT:**
>Input 10 elements in the array :                                                                              
>element - 0 : 1                                                                                               
>element - 1 : 1                                                                                               
>element - 2 : 2                                                                                               
element - 3 : 3                                                                                               
element - 4 : 4                                                                                               
element - 5 : 5                                                                                               
element - 6 : 6                                                                                               
element - 7 : 7                                                                                               
element - 8 : 8                                                                                               
element - 9 : 9                                                                                               
                                                                  >                                            
>Elements in array are: 1  1  2  3  4  5  6  7  8  9

**19)Program to Enter and Display Elements of 2D Array**
```C
#include<stdio.h>
int main(){
   /* 2D array declaration*/
   int disp[2][3];
   /*Counter variables for the loop*/
   int i, j;
   for(i=0; i<2; i++) {
      for(j=0;j<3;j++) {
         printf("Enter value for disp[%d][%d]:", i, j);
         scanf("%d", &disp[i][j]);
      }
   }
   //Displaying array elements
   printf("Two Dimensional array elements:\n");
   for(i=0; i<2; i++) {
      for(j=0;j<3;j++) {
         printf("%d ", disp[i][j]);
         if(j==2){
            printf("\n");
         }
      }
   }
   return 0;
}
```
**OUTPUT:**
>Enter value for disp[0][0]:1
Enter value for disp[0][1]:2
Enter value for disp[0][2]:3
Enter value for disp[1][0]:4
Enter value for disp[1][1]:5
Enter value for disp[1][2]:6
Two Dimensional array elements:
1 2 3 
4 5 6 

**20) Program to add to Matrix:**
```#include<stdio.h>

int a[3][3], b[3][3],c[3][3], i ,j;
int main(){
printf("Welcome to the Matrix Program");

printf("Enter the value of matrix A");
for(i=0;i<3;i++){
for(j=0;j<3;j++){
scanf("%d",&a[i][j]);
}}


printf("Enter the value of matrix B");
for(i=0;i<3;i++){
for(j=0;j<3;j++){
scanf("%d",&b[i][j]);
}}

printf("You have entered all the values of the matrix\n");
printf("Now the program is displaying the addition of  matrix");

for(i=0;i<3;i++){
for(j=0;j<3;j++){
c[i][j] = b[i][j] + a[i][j];
}}

for(i=0;i<3;i++){
for(j=0;j<3;j++){

printf("%d\t",c[i][j]);
}
printf("\n");}


}
```

**OUTPUT:**
> Welcome to the Matrix ProgramEnter the value of matrix A
> 23
> 67
> 12
> 89
> 23
> 78
> 12
> 65
> 23
> Enter the value of matrix B45
> 67
> 89
> 23
> 62
> 48
> 69
> 52
> 84
> You have entered all the values of the matrix
> Now the program is displaying the addition of  matrix
> 68      134     101
> 112     85      126
> 81      117     107

**21)Program to Display Transpose of Matrix:**

```#include<stdio.h>

int a[3][3],c[3][3], i ,j;
int main(){
printf("Welcome to the Matrix Transpose Program");

printf("Enter the value of matrix");
for(i=0;i<3;i++){
for(j=0;j<3;j++){
scanf("%d",&a[i][j]);
}}

for(i=0;i<3;i++){
for(j=0;j<3;j++){

printf("%d\t",a[i][j]);
}

printf("You have entered all the values of the matrix\n");
printf("Now the program is displaying the transpose of matrix\n");

for(i=0;i<3;i++){
for(j=0;j<3;j++){
c[j][i] = a[i][j];
}}

for(i=0;i<3;i++){
for(j=0;j<3;j++){

printf("%d\t",c[i][j]);
}
printf("\n");}


}
}
```

**OUTPUT:**
> Welcome to the Matrix Transpose ProgramEnter the value of matrix34
> 34
> 56
> 625
> 536
> 75
> 68
> 97
> 07
> You have entered all the values of the matrix
> Now the program is displaying the transpose of matrix
> 34      625     68
> 34      536     97
> 56      75      7


**22)Program for Subtraction of 2 Matrix:**
```#include<stdio.h>

int a[3][3], b[3][3],c[3][3], i ,j;
int main(){
printf("Welcome to the Matrix Program");

printf("Enter the value of matrix A");
for(i=0;i<3;i++){
for(j=0;j<3;j++){
scanf("%d",&a[i][j]);
}}


printf("Enter the value of matrix B");
for(i=0;i<3;i++){
for(j=0;j<3;j++){
scanf("%d",&b[i][j]);
}}

printf("You have entered all the values of the matrix\n");
printf("Now the program is displaying the addition of  matrix");

for(i=0;i<3;i++){
for(j=0;j<3;j++){
c[i][j] = b[i][j] - a[i][j];
}}

for(i=0;i<3;i++){
for(j=0;j<3;j++){

printf("%d\t",c[i][j]);
}
printf("\n");}


}
```

**OUTPUT:**
> Welcome to the Matrix ProgramEnter the value of matrix A
> 34
> 26
> 73
> 84
> 53
> 15
> 73
> 86
> 24
> Enter the value of matrix B
> 1
> 57
> 43
> 57
> 33
> 10
> 24
> 46
> 13
> You have entered all the values of the matrix
> Now the program is displaying the addition of  matrix-33        31      -30
> -27     -20     -5
> -49     -40     -11

**23)Program to Find Multiplication of Matrix**
```C
    #include <stdio.h>
    int main()
    {
        int a[10][10], b[10][10], result[10][10], r1, c1, r2, c2, i, j, k;
        printf("Enter rows and column for first matrix: ");
        scanf("%d %d", &r1, &c1);
        printf("Enter rows and column for second matrix: ");
        scanf("%d %d",&r2, &c2);
        // Column of first matrix should be equal to column of second matrix and
        while (c1 != r2)
        {
            printf("Error! column of first matrix not equal to row of second.\n\n");
            printf("Enter rows and column for first matrix: ");
            scanf("%d %d", &r1, &c1);
            printf("Enter rows and column for second matrix: ");
            scanf("%d %d",&r2, &c2);
        }
        // Storing elements of first matrix.
        printf("\nEnter elements of matrix 1:\n");
        for(i=0; i<r1; ++i)
            for(j=0; j<c1; ++j)
            {
                printf("Enter elements a%d%d: ",i+1, j+1);
                scanf("%d", &a[i][j]);
            }
        // Storing elements of second matrix.
        printf("\nEnter elements of matrix 2:\n");
        for(i=0; i<r2; ++i)
            for(j=0; j<c2; ++j)
            {
                printf("Enter elements b%d%d: ",i+1, j+1);
                scanf("%d",&b[i][j]);
            }
        // Initializing all elements of result matrix to 0
        for(i=0; i<r1; ++i)
            for(j=0; j<c2; ++j)
            {
                result[i][j] = 0;
            }
        // Multiplying matrices a and b and
        // storing result in result matrix
        for(i=0; i<r1; ++i)
            for(j=0; j<c2; ++j)
                for(k=0; k<c1; ++k)
                {
                    result[i][j]+=a[i][k]*b[k][j];
                }
        // Displaying the result
        printf("\nOutput Matrix:\n");
        for(i=0; i<r1; ++i)
            for(j=0; j<c2; ++j)
            {
                printf("%d  ", result[i][j]);
                if(j == c2-1)
                    printf("\n\n");
            }
        return 0;
    }
```
    
**OUTPUT:**
>Enter rows and column for first matrix: 3
2
Enter rows and column for second matrix: 3
2
Error! column of first matrix not equal to row of second.
>
>Enter rows and column for first matrix: 2
3
>Enter rows and column for second matrix: 3
2
>
>Enter elements of matrix 1:
Enter elements a11: 3
Enter elements a12: -2
Enter elements a13: 5
Enter elements a21: 3
Enter elements a22: 0
Enter elements a23: 4
>
>Enter elements of matrix 2:
Enter elements b11: 2
Enter elements b12: 3
Enter elements b21: -9
Enter elements b22: 0
>Enter elements b31: 0
>Enter elements b32: 4
>
>Output Matrix:
>24  29
>
>6  25

**24)Program to find square of a number using function**
```#include <stdio.h>
int num,a;
int square(int num);

void main(){
printf("Welcome to the program to find the square of a number\n");
printf("Input the number you want to print:\n")
scanf("%d", &num);
square(num);
}

int square(int a)
{
printf("The Answer is :%d\n",a*a);
}
```

**OUTPUT:**

> Welcome to the program to find the square of a number
> Input the number you want to find square of:
> 3
> The Answer is:9


**25)Program to swap two numbers by call by value**

```#include<stdio.h>
void swap(int a,int b);
void main()
{
int x,y;
printf("\n Enter value for x:");
scanf("%d",&x);
printf("\n Enter value for y:");
scanf("%d",&y);
printf("\n Before calling swap functin\n");
printf("\n Value of x=%d,Value of y=%d\n",x,y);
swap(x,y);
printf("\n After returning from swap function");
printf("\n Value of x=%d,value of y=%d\n",x,y);
}
void swap(int a,int b)
{
int temp;
printf("\n Inside the function \n");
printf("\n Value of a=%d,Value of b=%d before swaping\n",a,b);
temp=a;
a=b;
b=temp;
printf("\n Value of a=%d,Value of b=%d after swaping\n",a,b);
}
```
**OUTPUT:**

>  Enter value for x:45
> 
>  Enter value for y:56
> 
>  Before calling swap functin
> 
>  Value of x=45,Value of y=56
> 
>  Inside the function 
> 
>  Value of a=45,Value of b=56 before swaping
> 
>  Value of a=56,Value of b=45 after swaping
> 
>  After returning from swap function
>  Value of x=45,value of y=56
 

**26)Program to swap two numbers by call by reference**
 
```#include<stdio.h>
void swap(int *,int *);
void main()
{
int x,y;
printf("\n Enter value for x:");
scanf("%d",&x);
printf("\n Enter value for y:");
scanf("%d",&y);
printf("\n Before calling swap functin\n");
printf("\n Value of x=%d,Value of y=%d\n",x,y);
swap(&x,&y);
printf("\n After returning from swap function");
printf("\n Value of x=%d,value of y=%d\n",x,y);
}
void swap(int *a,int *b)
{
int temp;
printf("\n Inside the function \n");
printf("\n Value of a=%d,Value of b=%d before swaping\n",*a,*b);
temp=*a;
*a=*b;
*b=temp;
printf("\n Value of a=%d,Value of b=%d after swaping\n",*a,*b);
}
```

 
 **OUTPUT:**
 
 >  Enter value for x:23
> 
>  Enter value for y:45
> 
>  Before calling swap functin
> 
>  Value of x=23,Value of y=45
> 
>  Inside the function 
> 
>  Value of a=23,Value of b=45 before swaping
> 
>  Value of a=45,Value of b=23 after swaping
> 
>  After returning from swap function
>  Value of x=45,value of y=23
> 

**27)Program to Find factorial of a number using recursion:**
```#include <stdio.h>
int count = 1, num;
int multiply(int num);

int main(){
printf("Welcome to the program to find factorial by recursion");
printf("Write the number:\n");
scanf("%d",&num);
multiply(num);
printf("The facorial is %d",count);
}

int multiply(int num){
 count = count * num;
if(num>1){
 multiply(num - 1);
}
return count;}
```
**OUTPUT:**
> Welcome to the program to find factorial by recursionWrite the number:
> 8
> The facorial is 40320

**28)Program to Find fibonacci series using recursion:**

```#include <stdio.h>
int count, num1, num2, b;
int add(int num1,
```

**OUTPUT:**

> Welcome to the program to write the fibonacci series by recursion
> Write the first and second number of the series
> 2
> 3
> How many terms you want in the fibonacci series
> 20
> The fibonacci series is
> 2
> 3
> 5
> 8
> 13
> 21
> 34
> 55
> 89
> 144
> 233
> 377
> 610
> 987
> 1597
> 2584
> 4181
> 6765
> 10946
> 17711

**29)Program to add elements to a structure and display them**
```C
#include <stdio.h>
struct student
{
    char name[50];
    int roll;
    float marks;
} s[10];
int main()
{
    int i;
    printf("Enter information of students:\n");
    // storing information
    for(i=0; i<10; ++i)
    {
        s[i].roll = i+1;
        printf("\nFor roll number%d,\n",s[i].roll);
        printf("Enter name: ");
        scanf("%s",s[i].name);
        printf("Enter marks: ");
        scanf("%f",&s[i].marks);
        printf("\n");
    }
        printf("Displaying Information:\n\n");
    // displaying information
    for(i=0; i<10; ++i)
    {
        printf("\nRoll number: %d\n",i+1);
        printf("Name: ");
        puts(s[i].name);
        printf("Marks: %.1f",s[i].marks);
        printf("\n");
    }
    return 0;
}
 
```
**OUTPUT:**
>Enter information of students: 
>
>For roll number1,
>Enter name: Tom
>Enter marks: 98
>
>For roll number2,
>Enter name: Jerry
>Enter marks: 89
>.
>.
>.
>Displaying Information:
>Roll number: 1
>Name: Tom
>Marks: 98
>.
>.
>.

**30) Array using structure**
```C
#include <stdio.h>
#include <string.h>
 
struct student 
{
     int id;
     char name[30];
     float percentage;
};
 
int main() 
{
     int i;
     struct student record[2];
 
     // 1st student's record
     record[0].id=1;
     strcpy(record[0].name, "Raju");
     record[0].percentage = 86.5;
 
     // 2nd student's record         
     record[1].id=2;
     strcpy(record[1].name, "Surendren");
     record[1].percentage = 90.5;
 
     // 3rd student's record
     record[2].id=3;
     strcpy(record[2].name, "Thiyagu");
     record[2].percentage = 81.5;
 
     for(i=0; i<3; i++)
     {
         printf("     Records of STUDENT : %d \n", i+1);
         printf(" Id is: %d \n", record[i].id);
         printf(" Name is: %s \n", record[i].name);
         printf(" Percentage is: %f\n\n",record[i].percentage);
     }
     return 0;
}
```
**OUTPUT:**
>Records of STUDENT : 1
>Id is: 1
>Name is: Raju
>Percentage is: 86.500000
>
>Records of STUDENT : 2
>Id is: 2
>Name is: Surendren
>Percentage is: 90.500000
>
>Records of STUDENT : 3
Id is: 3
>Name is: Thiyagu
>Percentage is: 81.500000

**31)Pointer or variable**
```C
#include <stdio.h>

int main () {

   int  var = 20;   /* actual variable declaration */
   int  *ip;        /* pointer variable declaration */

   ip = &var;  /* store address of var in pointer variable*/

   printf("Address of var variable: %x\n", &var  );

   /* address stored in pointer variable */
   printf("Address stored in ip variable: %x\n", ip );

   /* access the value using the pointer */
   printf("Value of *ip variable: %d\n", *ip );

   return 0;
}
```
**OUTPUT**
>Address of var variable: bffd8b3c
>Address stored in ip variable: bffd8b3c
>Value of *ip variable: 20


