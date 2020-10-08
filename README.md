# Calculate-new-salary
#include <stdio.h>
#include <stdlib.h>


int main()
{
    char Ename[10];
    
    int bsal,nsal;
    
    float increment;
    
    printf("Enter Employee Name here\n");
    
    scanf("%s",&Ename);
    
    printf("Enter Empolyee basic salary here");
    
    scanf("%d",&bsal);

    if (bsal<5000)
        increment=(0.05*bsal);
    else
        if (bsal<10000)
            increment=(0.10*bsal);
        else
            increment=(0.15*bsal);
    nsal=bsal+increment;
    printf("Employee name is %s and his salary is %d",Ename,nsal);

    return 0;
}
