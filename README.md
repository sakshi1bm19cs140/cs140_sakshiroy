# cs140_sakshiroy
#include<stdio.h>
int main()
{
    int z=1;
    int x;
    int y;
    printf("Enter two numbers\n");
    scanf("%d%d",&x,&y);
    while(z!=0)
    {
        int i;
        printf("\nPress: 1 for Addition\n2 for substraction\n3 for multiplication\n4 for division\n5 to compare\n6 to modules\n7 for remainder\n8 to exit\n");
        scanf("%d",&i);
        if(i==1)
        printf("%d",x+y);
        else if(i==2)
        printf("%d",x-y);
        else if(i==3)
        printf("%d",x*y);
        else if(i==4)
        printf("%d",x/y);
        else if(i==5)
        {
            if(x==y)
            {
                printf("The numbers are equal");
            }
            else
            {
                if(x>y)
                printf("x is greater\n");
                else
                printf("y is greater");
            }
        }
        else if(i==6)
        printf("%d",abs(x+y));
        else if(i==7)
        printf("%d",x%y);
        else if(i==8)
        {
            printf("Thank You");
            z=0;
        }
        else
        {
            printf("Please select a number between 1 to 8\n");
        }
    }
    return 0:
}

/*Second Program*/

#include<stdio.h>
int sumaver(int x,int y)
{
    int sum=x+y;
    int avg=sum/2;
    printf("Sum is %d\n",sum);
    return avg;
}
int printeven(int x , int y)
{
    if(x%2==0)
    {
        printf("\n%d is even",x);

    }
    if(y%2==0)
    {
            printf("\n%d is even",y);
    }
}
int main()
{
    int x,y,z,avg;
    printf("Enter three numbers: ");
    scanf("%d%d%d",&x,&y,&z);
    if(x>y && x>z)
    {
        if(y>z)
        {
            avg=sumaver(x,y);

            printf("%d is the avg\n",avg);
            printeven(x,y);
        }
        else
        {
            avg=sumaver(x,z);

            printf("%d is the avg\n",avg);
            printeven(x,z);
        }
    }
    else if(y>z && y>x)
    {
        if(z>x)
        {
            avg=sumaver(y,z);
            printf("%d is the avg",avg);
            printeven(y,z);

        }
        else
        {
            avg=sumaver(x,y);
            printf("%d is the avg\n",avg);
            printeven(x,y);
        }

    }
    else
    {
        if(x>y)
        {
            avg=sumaver(x,z);
            printf("%d is the avg\n",avg);
            printeven(x,z);
        }
        else
        {
            avg=sumaver(y,z);
            printf("%d is the avg\n",avg);
            printeven(y,z);

        }
    }
    return 0;
}  
