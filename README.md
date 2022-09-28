# csa0378_dscrt_323
#include<stdio.h>
long int multiplyNumbers(int n);
int main() {
    int n;
    printf("Enter a positive integer: ");
    scanf("%d",&n);
    printf("Factorial of %d = %ld", n, multiplyNumbers(n));
    return 0;
}

long int multiplyNumbers(int n) {
    if (n>=1)
        return n*multiplyNumbers(n-1);
    else
        return 1;
}

![fact_rec](https://user-images.githubusercontent.com/100762152/192726859-999aef6a-d6c1-4c03-aebf-d118815e4af2.png)
#matrix_c
#include<stdio.h>
int main(){
    int a[10][10],b[10][10],c[10][10],n,i,j,k;
    
    printf("Enter the value of N (N <= 10): ");
    scanf("%d",&n);
    printf("Enter the elements of Matrix-A: \n");
    
    for(i=0;i<n;i++)
    {
        for(j=0;j<n;j++)
        {
            scanf("%d",&a[i][j]);
        }
    }
    
    printf("Enter the elements of Matrix-B: \n");
    
    for(i=0;i<n;i++)
    {
        for(j=0;j<n;j++)
        {
            scanf("%d",&b[i][j]);
        }
    }
    
    for(i=0;i<n;i++)
    {
        for(j=0;j<n;j++)
        {
            c[i][j]=0;
            for(k=0;k<n;k++)
            {
                c[i][j]+=a[i][k]*b[k][j];
            }
        }
    }
    
    printf("The product of the two matrices is: \n");
    for(i=0;i<n;i++)
    {
        for(j=0;j<n;j++)
        {
            printf("%d\t",c[i][j]);
        }
        printf("\n");
    }
    return 0;
}
![matrix_c](https://user-images.githubusercontent.com/100762152/192732254-0e53a8b5-a63f-489e-a7f4-e1b79441c2ed.png)
