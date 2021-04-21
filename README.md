# Chapter6
Exercises from Chapter 6 of the book "Practical C Programming"
## Exercise 6-1
```c
#include <stdio.h>
#include <math.h>
int main(void) {
float p1, q1, p2, q2, d, sump, sumq, r;

  printf("Enter p1: ");
  scanf("%f", &p1);

  printf("Enter q1: ");
  scanf("%f", &q1);

  printf("Enter p2: ");
  scanf("%f", &p2);

  printf("Enter q2: ");
  scanf("%f", &q2);

sump = (p2 - p1);
sumq = (q2 - q1);

d = pow(sump, 2) + pow(sumq, 2);

r = sqrt(d);

printf("Distance between 2 points is %f", r);

return 0;
}
```
## Exercise 6-2:
```c
#include <stdio.h>
int main(void) {
int i;

  printf("Introduce a number: ");
  scanf("%d", &i);

if (i >= 0 && i <=60){ 
  printf("F"); 
   
}
else if (i >= 61 && i <=70){ 
  printf("D"); 
   
}
else if (i >= 71 && i <=80){ 
  printf("C");    
   
}
else if (i >= 81 && i <=90){ 
  printf("C");    
   
}
else if (i >= 91 && i <=100){ 
  printf("A");    
   
}

return 0;
}
```
## Exercise 6-3:
```c
int main(void) {
int a, grade;
  
  printf("Introduce grade: ");
  scanf("%d", &a);

grade = a % 10;

if (a <=60){
  printf("F");
}

else if(a <= 70 && a >= 61){

  if (grade <= 3 && grade >= 1)
    {printf("D-");}

  else if (grade <= 7 && grade >= 4)
    {printf("D");}
    
  else if ((grade >= 8 && grade <= 9) || grade == 0 )
    {printf("D+");}
    
  else
    {printf("ERROR");}
}

else if(a <= 80 && a >= 71){

if(grade <= 3 && grade >= 1){
  printf("C-");
}
else if(grade <= 7 && grade >= 4){
  printf("C");
}
else if((grade >= 8 && grade <= 9) || grade==0){
  printf("C+");
}
else {printf("ERROR");
}
} else if(a <= 90 && a >= 81){

if(grade <=3 && grade >=1){
  printf("B-");
}
else if(grade <=7 && grade >=4){
  printf("B");
}
else if((grade >= 8 && grade <= 9) || grade==0){
  printf("B+");
}
else {printf("ERROR");
}
}

else if(a <= 100 && a >= 91){

if(grade <=3 && grade >=1){
  printf("A-");
}
else if(grade <=7 && grade >=4){
  printf("A");
}
else if((grade >= 8 && grade <= 9) || grade==0){
  printf("A+");
}
else {printf("ERROR");
}
}
return 0; }
```
## Exercise 6-4:
```c
#include<stdio.h>
#include<math.h>

int main(void){
float money1;
int leftquarters, leftdimes, leftnickels, quarters, dimes, nickels;

printf("Introduce amount of money: ");
scanf("%f", &money1);

int indmoney = money1 * 100;
quarters = indmoney / 25;
leftquarters = indmoney % 25;
dimes = leftquarters / 10;
leftdimes = leftquarters % 10;
nickels = leftdimes / 5;
leftnickels = leftdimes % 5;

printf("In %f$ there are %d quarters, %d dimes, %d nickels and %d pennies", money1, quarters, dimes, nickels, leftnickels);
```
## Exercise 6-5:
```c
#include<stdio.h>
#include<math.h>

int main(void){
int year, year1;

printf("Introduce a leap year: ");
scanf("%d", &year);

if ( ((year % 4) == 0 && (year % 100) != 0)|| (year % 400) == 0){
printf("Leap year");
}

else if ((year % 400) != 0 && (year % 100) == 0){
printf("Not a leap year");
}
else{
  printf("Introduced year %d is not leap year", year);
}

return 0;
}
```
## Exercise 6-6:
```c
#include<stdio.h>
#include<math.h>

int main(void){
float salary, nhours, hours, total, subtotal;

printf("Introduce salary (per hour):");
scanf("%f",&salary);

printf("Introduce worked hours (week):");
scanf("%f",&hours);

float mult = 1.5;

if (hours <= 40) {
  total = hours * salary;

}
else {
  nhours = hours - 40;
  total = 40 * salary;
  total += nhours * (salary + (salary/2));

}
printf("Weekly pay: $%f\n", total);

return 0; }
```
