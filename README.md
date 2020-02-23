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


#include <stdio.h>
/*
//Task 02 dated: 22/02/2020
int series (int size,int counter)
{    if(size==10)
    return 1;
    else {
        printf("%d \n",size+counter);
        return series(size+1,counter+1);
            }
}
int main()
{   
    int size=1;
    int counter=0;
    series(size,counter);
    return 0;
}
*/


/*
//task 01 dated: 22/02/2020
int PrintTable(int x)
{int n=4;
    if(x==4)
        return 0;
    else{
        printf("%d X %d = %d\n",n,x, x*n);
        return PrintTable(x+1);
    }
}
int main()
{   int num=1;
    PrintTable(num);
        return 0;
}
*/

//task 03: 23/02/2020
int main()
{
    int my2Darray[2][2];
for(int i=0;i<2;i++)
{   for(int j=0;j<2;j++)
        {printf("enter value for index %d %d: \n", i,j);
        scanf("%d",&my2Darray[i][j]);
        }
    }
    
    printf("now printing 2D matrix\n");
        printf("%d  %d \n",my2Darray[0][0],my2Darray[0][1]);
        printf("%d  %d \n",my2Darray[1][0],my2Darray[1][1]);
        
        //for(i=0;i<2;i++)
          //  {   for(j=0;j<2;j++)
            //    {printf("enter value for index %d %d: \n", i,j);

    
    return 0;
}
