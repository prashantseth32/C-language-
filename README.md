# C-language-
To find the Fibbonacci Series




#include <stdio.h>
int main(){
    int i,num, previous_sec=0,previous_fir=1,current;
    printf("enter Number to get fibbonacci series to that no.:\n");
    scanf("%d",&num);

    for(i=0;i<num;i++)
    {
        if(i==0)
        {
            printf("the series is:\n");
            printf("%d\n",previous_sec);
        }
        else if(i==1)
        {
            printf("%d\n",previous_fir);
        }
        else
        {
            current=previous_sec + previous_fir;
            printf("%d\n",current);
            previous_sec = previous_fir;
            previous_fir = current;
        }
    }
    return 0;

}
