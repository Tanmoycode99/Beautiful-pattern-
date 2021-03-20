// Beautiful-pattern-
//This program will take input from the user of its rows and columns.
//after taking input this program will print diamond shape patterns sequentially and iteratively in loop.
//This program will print step by step growth of a pattern.

#include <stdio.h>

int main()
{
	int n,i,j,x;
	printf("Enter the number of patterns and rows alltogether:");
	scanf("%d",&n);
	for(x=0;x<=n;x++)
	{
	for(i=0;i<=x;i++)
	{
		for(j=0;j<=2*x-1;j++)
		{
			if( j>=x-(i-1) && j<=x+(i-1))
			{
				printf("*");
			 }
			 else 
			 {
			 	printf(" ");
			  } 
		}
		printf("\n");
	}
	
    for(i=x;i>=0;i--)
	{
		for(j=2*x-1;j>=0;j--)
		{
			if(j>=x-(i-1) && j<=x+(i-1))
			{
				printf("*");
			 }
			 else 
			 {
			 	printf(" ");
			  } 
		}
		printf("\n");
	}
}
  return 0;
}
