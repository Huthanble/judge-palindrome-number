# judge-palindrome-number
回文数是指正序（从左向右）和倒序（从右向左）读都是一样的整数，比如7，1221，12321都是回文数，而1234不是回文数。 现在给出一些数，请你判断它们是不是回文数。
#include<stdio.h>
int main()
{
    int x,newed,t,n;
    while(scanf("%d",&x)!=EOF)
    {
        newed=0;
        n=x;
        do
        {
            newed=newed*10+x%10;
            x/=10;
        }while(x>0);
        if(n==newed)
            printf("Yes\n");
        else
            printf("No\n");
    }
    return 0;
}
