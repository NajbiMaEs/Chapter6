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
```
## Exercise 6-3:
```c
```
