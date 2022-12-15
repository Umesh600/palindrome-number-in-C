# palindrome-number-in-C
Write a c program to check number is palindrom or not.

#include <stdio.h>

int main() {
    
    int n,r,rev=0,temp;
    
    printf("Enter any number:");
    scanf("%d",&n);
    
    temp=n;
    
    while(n!=0)
    {
        r=n%10;
        rev=rev*10+r;
        n=n/10;
    }
    temp=rev;
    
    if(temp==rev)
    {
        printf(" number is palindrom");
    }
    else 
    {
        printf(" no is not palindrom");
    }
    
    return 0;
}
