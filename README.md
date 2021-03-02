# Chapter6

# First Exercise

 #include <stdio.h>
 
#include<math.h>


int main(void) {

 double x1;
 
 double x2;
 
 double y1;
 
 double y2;

 printf("Please insert, in this order, coordenates x1, x2, y1 and y2\n");
 
 scanf("%lf %lf %lf %lf", &x1, &x2, &y1, &y2);
 
 double firstdiff = (x1-x2);
 
 double firstsquare = pow(firstdiff, 2);
 
 double seconddiff = (y1-y2);
 
 double secondsquare = pow(seconddiff, 2);
 
 double sum = firstsquare + secondsquare;
 
 double distance = sqrt(sum);
 
 printf("The distance between those points is %lf", distance); 
 

  return 0;
  
}
