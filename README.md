# Aptech-PM-program
introductory classes to C

//user defined funtion to generate a table, function doesnt return a value
#include <stdio.h>
void table(int num)
{
    for(int i=1;i<=10;i++)
    {    printf("%d X %d = %d \n",num,i,num*i);   }
}

int main()
{
    int input=0;
    printf("Enter a number to generate a table \n");
    scanf("%d",&input);
    table(input);
    return 0;
}
