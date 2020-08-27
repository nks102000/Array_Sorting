# Array_Sorting
Selection sort
//1905622 - NITISH KUMAR SONTHALIA
//SORTING
#include <stdio.h>

int main()
{
    int i,n;  
 
     printf("Enter size of array: ");
    scanf("%d",&n);
    int a[100];
 
     printf("Enter %d elements in the array : ", n);
    for(i=0;i<n;i++)
    {
        scanf("%d", &a[i]);
    }
 
    printf("\nElements in array are: ");
    for(i=0;i<n;i++)
 
    {
        printf("%d  ", a[i]);
    }
    
     int j; 
   for (i = 0; i < n-1; i++)          
       for (j = 0; j < n-i-1; j++)  
           if (a[j] > a[j+1]){
            int temp = a[j]; 
            a[j]=a[j+1]; 
            a[j+1] = temp; 
           } 

    printf("\nElements in array are: ");
    for(i=0;i<n;i++)
 
    {
        printf("%d  ", a[i]);
    } 
    return 0;
}
