#include<stdio.h>
#include <stdlib.h>

int main()
{
	int i,j,k=0;
	int a[10] = {5, 9, 0, 1, 3, 6, 8, 7, 2, 4};

	for(i=0;i<9;i++)
		for(j=i+1;j<10;j++)
			if(a[i]>a[j])
			{
				k=a[i];a[i]=a[j];a[j]=k;
			}
		for(i=0;i<10;i++)
			printf("%3d",a[i]);
	printf("\n");
	system("pause");
	return 0;
}
