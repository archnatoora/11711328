# 11711328
/* 21. Ten students (a,b,c,d,e,f,g,h,i,j) are going to attend an event.
There are lots of gift shops, they all are going to the gift shops and randomly picking the gifts.
After picking the gifts they are randomly arriving in the billing counter. 
The accountant gives the preference to that student who has maximum number of gifts.
Create a C or Java program to define order of billed students? */

#include <stdio.h>
#include<stdlib.h> 
int main()
{
  int a[10], n=10, c, d,e, swap;
  char b[10];
  char A,B,C,D,E,F,G,H,I,J;
  printf("Students are attending an event and buying gifts:\n");
	c=0;
	printf("Enter the number of gifts for students A \n");
   scanf("%d", &a[c]);
   c=c+1;
   printf("Enter the number of gifts for students B \n");
   scanf("%d", &a[c]);
   c=c+1;
   printf("Enter the number of gifts for students C \n");
   scanf("%d", &a[c]);
   c=c+1;
   printf("Enter the number of gifts for students D \n");
   scanf("%d", &a[c]);
   c=c+1;
   printf("Enter the number of gifts for students E \n");
   scanf("%d", &a[c]);
   c=c+1;
   printf("Enter the number of gifts for students F \n");
   scanf("%d", &a[c]);
   c=c+1;
   printf("Enter the number of gifts for students G \n");
   scanf("%d", &a[c]);
   c=c+1;
   printf("Enter the number of gifts for students H \n");
   scanf("%d", &a[c]);
   c=c+1;
   printf("Enter the number of gifts for students I \n");
   scanf("%d", &a[c]);
   c=c+1;
   printf("Enter the number of gifts for students J \n");
   scanf("%d", &a[c]);
   
   for (c = 0 ; c < ( n - 1 ); c++)
  {
    for (d = 0 ; d < n - c - 1; d++)
    {
      if (a[d] < a[d+1]) 
      {
        swap       = a[d];
        a[d]   = a[d+1];
        a[d+1] = swap;
      }
    }
  }
  printf("Accountant first gives the preference who has maximum gifts!!\n");
  printf("Here is the order of billed students:\n");
     for (c = 0; c < n; c++)
     printf("%d\n", a[c]);

 
  return 0;
}
