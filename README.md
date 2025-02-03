#include <stdio.h>
int main()
{
  int a,b,c;
  scanf("%d %d %d",&a,&b,&c);
  if(c==1)
  {
    c=a+b;
    printf("%d",c);
  }
  else if(c==2)
  {
    c=a-b;
    printf("%d",c);
  }
  else if(c==3)
  {
    c=a*b;
    printf("%d",c);
  }
  else if(c==4)
  {
    c=a/b;
    printf("%d",c);
  }
  else
  {
  printf("Invalid Input");
  }
  return 0;
}
