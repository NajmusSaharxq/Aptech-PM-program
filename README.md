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



//user defined funtion to generate a table, function returns value
//last value is not being displayed
#include <stdio.h>
int table(int num)
{
    int lastProduct,prod=0;
    for(int i=1;i<=10;i++)
    {    printf("%d X %d = %d \n",num,i,num*i);   

     if (i==10)
     { printf("%d %d \n",i,num);
     prod=num*i;
        return(prod);
    }}
   
}

int main()
{
    int input,output=0;
    printf("Enter a number to generate a table \n");
    scanf("%d",&input);
    output=(table(input));
    printf("last product of counter and user's number input is: \n",output);
    return 0;
}
