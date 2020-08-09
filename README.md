#include<stdio.h>
#include<stdlib.h>
#include<string.h>
#include<math.h>
void main()
         {
               char ch1='b';
               int R,T=0,i,M=0;
               char Name[20];
               char Names[5][20]={"Krishna","Malti","Shaurya","Rupan","Sunita"};
               printf("Enter Your name as you filled in the form\n");
               scanf("%s",Name);
               for(i=0;i<5;i++)
               {
                   if(strcmp(Name,Names[i])==0)
                    T+=1;}
                   if(T==1)
                    printf("Yes you can take the test\n");
                   else
                    {printf("Sorry you can't take any test.\n");
                   exit(1);}
                   printf("Here is your first question\n");
                   printf("Q1. One kilogram has \n ");
                   printf("1. 20nm   2. 100nm   3. 1000gm   4. none of the above");
                   printf("\n Please enter  1 or 2 or 3 or 4:\n");
                   scanf("%d",&R);
                   if(R==3) M+=5;
                   printf("Here is your second question");
                   printf("\n How many Continents are in the world?");
                   scanf("%d",&R);
                   if(R==6) M+=5;
                   printf("\nYour Total marks id %d",M);
               }


