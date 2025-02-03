#include <stdio.h>
int main()
{
  int amount=5000;
  printf("Enter 1: Account Balance\nEnter 2:Cash Withdrawl\nEnter 3:Cash Deposit\n");
  while(1)
  {
    printf("Enter you are choice(1 to 3):");
  int ch,rs;
  scanf(" %d",&ch);
  if(ch==1)
  {
    printf("Account balance:%d\n",amount);
  }
  else if(ch==2)
  {
    printf("Enter the Amount to Withdrawl: ");
    scanf("%d",&rs);
    if(rs>amount)
    {
      printf("Insufficient Balance\n");
    }
    else
    {
      amount-=rs;
      printf("Account balance:%d\n",amount);
    }
  }
  else if(ch==3)
  {
    printf("Enter the Amount to Deposit:");
    scanf("%d",&rs);
    amount+=rs;
    printf("Account Balance:%d\n",amount);
  }
  else 
  {
    printf("Invalid Choice");
  }
  printf("Do you want to continue(Type y to continue):");
  char d;
  scanf(" %c",&d);
  if (d!='y')
  {
  printf("Thank you!\n");
  break;
  }
 }
  return 0;
}
