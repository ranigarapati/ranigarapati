#include<stdio.h>
#include<string.h>
int main()
{
    char str[20];
    printf("enter a string");
    gets(str);
    int i, count1=0,count2=0,count3=0;
    for(i=0;str[1]!='\0';i++)
    {
        if(isupper(str[i]))
        {
            count1=count1+1;
        }
        else if(islower(str[i]))
        {
            count2=count2+1;
        }
        else if(isdigit(str[i]))
        {
            count3=count3+1;
        }
    }
    printf("count of uppercase characters=%d\n",count1);
    printf("count of lowercase characters=%d\n",count2);
    printf("count of digits=%d\n",count3);
    return 0;
}
enter a string Roja123
count of uppercase characters=1
count of lowercase characters=3
count of digits=3
