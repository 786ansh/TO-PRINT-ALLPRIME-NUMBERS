# TO-PRINT-ALLPRIME-NUMBERS



#include<stdio.h>
int prime(int);
void main()
{
    int n;
    printf("Enter the end value");
    scanf("%d",&n);
    prime(n);
}
int prime(int n)
{
    int i,j,count;

    printf("Prime Numbers are: \n");
    for(i=1; i<=n; i++)
    {
        count=0;
        for(j=1; j<=n; j++)
        {
            if(i%j==0)
                count++;
        }
        if(count==2)
            printf("%d " ,i);
    }
}
