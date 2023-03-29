#define _CRT_SECURE_NO_WARNINGS

#include<stdio.h>

int main(void) {

   int total;
   int hour, min, time;  

   scanf("%d %d", &hour, &min);

   scanf("%d", &time);

   total = hour * 60 + min + time; 

   hour = total / 60;   
   if (hour > 23) {
      hour -= 24;   
      min = total % 60;  

      printf("%d %d", hour, min);
   }

   else {
      min = total % 60;
      printf("%d %d", hour, min);
   }
   return 0;
}
