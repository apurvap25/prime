# prime
#include <stdio.h>
int Prime(int n)
{
  int i;
  for (i=2; i <n;i++)
  {
    if(n%i==0)
    break;
  }
  if (i==n)
      return n ;
      else
      return 0;
}


int main(void) {
  int start,end,i;
  printf("enter range");
  scanf("%d%d",&start,&end);
  printf("prime numbers between %d and %d",start,end);
  for (i=start;i<=end;i++)
  {
    if(Prime(i))
    printf("\n %d",i);
  }

  
  return 0;
}
