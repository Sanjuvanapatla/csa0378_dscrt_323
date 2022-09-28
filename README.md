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
