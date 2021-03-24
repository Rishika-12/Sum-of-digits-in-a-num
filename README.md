# Sum-of-digits-in-a-num

#include <stdio.h>

int main()
{
    printf("ENTER THE NUM:");
    int num;
    scanf("%d",&num);
    printf("The sum of digits is %d",sumofdigit(num));
    return 0;
}
int sumofdigit(int n){
    if (n==0)
        return 0;
    else 
        return(n%10+sumofdigit(n/10));
}
