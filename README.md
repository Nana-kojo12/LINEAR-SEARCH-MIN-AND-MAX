include <stdio.h>
#include <stdlib.h>

#define MaxSize 500000
int main()
 
{ 
  int arr[MaxSize];
  int i,max,min,size; 
  /*Input size of the array*/ 
    printf("\nEnter the size of the array:\n"); 
    scanf("%d",&size);
    
    /*Input the elements in the array*/
    printf("Enter elements in the array:");
    for(i=0; i<size;i++)
    {
    	scanf("%d", arr[i]);
	}


	max=arr[0];
	min=arr[0];

	for(i=1; i<size; i++)


	if(arr[i]>max)
	{
		max=arr[i];
	}
	if (arr[i]<min)
	{
		min=arr[i];

    }
	printf("Maximum element=%d\n",max);
	printf("Minimun element =%d",min);


	return 0;
}

