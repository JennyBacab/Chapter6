## Chapter6

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

# Second Exercise

#include <stdio.h>

#include<math.h>


int main(void) {

  int numgrade;
  
 printf("This program converts numeric grades to letter grades. Please insert a numeric grade\n");
 
 scanf("%int", &numgrade);
 
 if (numgrade <=60){


    printf("Letter grade is F\n");
    
} else if (numgrade>=61 && numgrade<=70){

    printf("Letter grade is D\n");
    
} else if (numgrade>=70 && numgrade<=80){

    printf("Letter grade is C\n");
    
} else if (numgrade>=81 && numgrade<=90){

    printf("Letter grade is B\n");
    
} else if (numgrade>=90 && numgrade<=100){

    printf("Letter grade is A\n");
    
}

return 0;

}

# Third Exercise

#include <stdio.h>

int main(void){

float numgrade;

printf("This program converts numeric grades to letter grades. Please insert a numeric grade\n");

scanf("%f",&numgrade);


if (numgrade <=60){


    printf("Letter grade is F\n");
    
} else if (numgrade>=61 && numgrade<=63){

    printf("Letter grade is D-\n");
    
} else if (numgrade>=64 && numgrade<=67){

    printf("Letter grade is D\n");
    
} else if (numgrade>=68 && numgrade<=70){

    printf("Letter grade is D+\n");
    
} else if (numgrade>=71 && numgrade<=73){

    printf("Letter grade is C-\n");
    
} else if (numgrade>=74 && numgrade<=77){

    printf("Letter grade  is C\n");
    
} else if (numgrade>=78 && numgrade<=80){

    printf("Letter grade is C+\n");
    
} else if (numgrade>=81 && numgrade<=83){

    printf("Leter grade is B-\n");
    
} else if (numgrade>=84 && numgrade<=87){

    printf("Letter grade is B\n");
    
} else if (numgrade>=88 && numgrade<=90){

    printf("Letter grade is B+\n");
    
} else if (numgrade>=91 && numgrade<=93){

    printf("Letter grade is A-\n");
    
} else if (numgrade>=94 && numgrade<=97){

    printf("Letter grade is A\n");
    
} else if (numgrade>=98 && numgrade<=100){

    printf("Letter grade is A+\n");
    
}

return 0;

}

# Fourth Exercise

#include <stdio.h>


int main(void){

 float moneydollars;
 
 printf("Please insert the money quantity in dollars\n");
 

 scanf("%f", &moneydollars);
 
 int money = moneydollars* 100;
 

 int quarters = money/25;
 
 int moneyleft = money%25;
 
 int dimes = moneyleft/10;
 
 int moneystillleft = moneyleft%10;
 
 int nickels = moneystillleft/5;
 
 int lastmoney = moneystillleft%5;
 
  
  printf("The money can be divided into %i quarter(s), %i dime(s), %i nickel(s) and %i penny/pennies\n", quarters, dimes, nickels, lastmoney);
  


return 0;


} 

# Exercise 5
#include <stdio.h>


int main(void) {

  int year;
  
  printf("This program will tell you if a year is a leap year\n");
  
  printf("Please insert a year\n");
  
  scanf("%i", &year);
  
  int test100 = year%100;
  
  int test400 = year%400;
  
  int test4 = year%4;
  
  if(test4!=0){
  
    printf("%i is not a leap year", year);
    
  }
  
  else if ((test100 == 0)&&(test400!=0)){
  
  printf("%i is not a leap year", year);
  
  }
  
  else
  
  {
  
  printf("%i is a leap year", year);
  
  }
  
  return 0;
  
}

# Exercise 6

#include <stdio.h>


int main(void) {

  float hours;
  
  float hourlywage;
  
  float weeklypay;
  
  int extratime;
  
  printf("This program will tell you the weekly pay of an employee given their hourly salary and hours worked\n");
  
  printf("Please insert worker's hourly wage\n");
  
  scanf("%f", &hourlywage);
  
  printf("Please insert number of hours worked\n");
  
  scanf("%f", &hours);
  
  if(hours<=40){
  
  weeklypay = hourlywage* hours;
  
  printf("The weekly pay is %f", weeklypay);
  
  }
  
  else{
  
  extratime = hours-40;
  
  weeklypay = hourlywage* 40 + extratime* hourlywage* 1.5;
  
  printf("The weekly pay is %f", weeklypay);
  
  }


  return 0;
  
}

# Exercise 7 - Original

#include <stdio.h>


int main(void) {

  int number;
  
  printf("This program will tell you if a number is a multiple of five, a multiple of two, or a multiple of both\n");
  
  scanf("%i", &number);
  
  int mult5 = number%5;
  
  int mult2 = number%2;
  
  if ((mult5==0)&&(mult2==0)){
  
    printf("%i is both a multiple of both 5 and 2",number);
    
  }
  else if (mult2==0){
  
    printf("%i is a multiple of 2 but not of five", number);
    
  }
  
  else if(mult5==0){
  
    printf("%i is a multiple of five but not of two", number);
    
  }
  
  else{
  
    printf("%i is not a multiple of neither two nor five",number);
    
  }
  

  return 0;
  
}
