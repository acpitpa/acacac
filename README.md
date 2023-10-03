# acacac

#include <stdio.h>
#include <math.h>

void main()
{
    int a,b,c;
    float x1, x2;
    
    printf("Enter your coefficients:");
    scanf("%d %d %d", &a, &b, &c);
    puts("Roots of the equation");
    
    x1=(-b+sqrt((pow(b,2))-(4*a*c)))/(2*a);
    x2=(-b-sqrt((pow(b,2))-(4*a*c)))/(2*a);
    
    
    switch (a) {
        case 0: printf(""); break;
        case 1: printf("x^2"); break;
        case -1: printf("-x^2"); break;
        
        default: printf("%dx^2", a);
    }
    
    if(b>0) printf("+");
    
    switch (b) {
        case 0: printf(""); break;
        case 1: printf("x"); break;
        case -1: printf("-x"); break;
        
        default: printf("%dx^2", b);
    }
  
  
    printf("%.2f,%.2f", x1, x2);

  
}
