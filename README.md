# Fraction
#include<stdio.h>
void main()
{
char ch;
printf("Enter any character (+,-,*,/)");
scanf("%c",&ch);
int n1,add1,add2,sub1,mul1,div1,sub2,mul2,div2,a,b;
printf("Enter first  numerator");
scanf("%d",&n1);
int d1;
printf("Enter first  denominator");
scanf("%d",&d1);
int n2;
printf("Enter second  numerator");
scanf("%d",&n2);
int d2;
printf("Enter second  denominator");
scanf("%d",&d2);

switch (ch)
{
case '+':
if(d1==d2)
{
a=(n1+n2);
b=d1;
printf("The addition of equation=%d/%d ",a,b);
}
else{
add1=((n1*d1)+(n2*d2));
add2=(d1*d2);
printf("The addition of equation=%d/%d ",add1,add2);
}
break;

case '-':
if(d1==d2)
{
a=(n1-n2);
b=d1;
printf("The addition of equation=%d/%d ",a,b);
}
else
{
sub1=((n1*d1)-(n2*d2));
sub2=(d1*d2);
printf("The substraction of equation=%d/%d", sub1,sub2);
}
break;

case '*':
mul1=(n1*n2);
mul2=(d1*d2);
printf("The multiplication of equation=%d/%d", mul1,mul2);
break;

case '/':
div1=(n1*d2);
div2=(d1*n2);
printf("The division of equation=%d", div1/div2);
break;


}



}
