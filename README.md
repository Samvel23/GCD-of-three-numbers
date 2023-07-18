#include <stdio.h>
int main()
{
int n1 = 0;
int n2 = 0;
int n3 = 0;
printf("Enter First Number:");
scanf("%d", &n1);
printf("Enter Second Number:");
scanf("%d", &n2);
printf("Enter Third Number:");
scanf("%d", &n3);
int min = 0;
if(n1 < n2 && n1 < n3){
  min = n1;
}else if(n2 < n1 && n2 < n3){
  min = n2;
}else{
  min = n3;
}
int i = 1;
int maxYndBaj = 0;
while(i != min){
  if(n1 % i == 0 && n2 % i == 0 && n3 % i == 0 && n3 % i == 0){
maxYndBaj = i;
  }
  i++;
}
printf("GCD = %d", maxYndBaj);
}
