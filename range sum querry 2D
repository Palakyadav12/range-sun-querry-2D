#include<conio.h>
#include<stdio.h>
void main()
{
    int a[10][10],i,j,r,c,r1,r2,c1,c2,sum=0,p[100][100];
    printf("enter the total no. of rows and column:-\n");
    printf("row:");
    scanf("%d",&r);
    printf("column:");
    scanf("%d",&c);
    for(i=0;i<r;i++)
    {
        for(j=0;j<c;j++)
        {
            printf("enter element:");
            scanf("%d",&a[i][j]);
        }
    }
    printf("the given array is:-\n ");
     for(i=0;i<r;i++)
    {
        printf("\n");
        for(j=0;j<c;j++)
        {
            printf("%d\t",a[i][j]);
        }
    }
    printf("\nenter the details to calculate the sum of a region in a given 2D array:-");
    printf("\nenter starting block:");
    printf("\nrow:");
    scanf("%d",&r1);
    printf("column:");
    scanf("%d",&c1);
    printf("enter ending block:");
    printf("\nrow:");
    scanf("%d",&r2);
    printf("column:");
    scanf("%d",&c2);
    for(i=0;i<=r;i++)
    {
        p[i][0]=0;
    }
    for(j=1;j<=c;j++)
    {
        p[0][j]=0;
    }
    for(i=1;i<=r;i++)
    {
        for(j=1;j<=c;j++)
        {
        p[i][j]=a[i-1][j-1]+p[i-1][j]+p[i][j-1]-p[i-1][j-1];
        }
    }
    sum = p[r2+1][c2+1]-p[r2+1][c1]-p[r1][c2+1]+p[r1][c1];
    //or without using prifix sum:-
    // for(i=r1;i<=r2;i++)
    // {
    //     for(j=c1;j<=c2;j++)
    //     {
    //         sum=sum+a[i][j];
    //     }
    // }
    printf("sum is %d",sum);
    getch();
}
