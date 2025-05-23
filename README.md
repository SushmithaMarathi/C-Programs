# C-Programs
//WRITE A SIMPLE C PROGRAM TO TAKE ARRAY SIZE AND ARRAY ELEMENTS FROM USER AS [1 2 3 4 5 6 7 8 9 10] AND PRINT ARRAY AS 2 4 6 8 10 9 7 5 3 1
#include <stdio.h>
int main() 
{
    int  size,i;
    printf("entersize of array:\n ",size);
    scanf("%d",&size);
    printf("enter array elements:\n");
    char arr[size];
    int even[5],odd[5],eIndex = 0, oIndex = 0;
    for(i=0;i<10;i++)
{
    scanf("%d",&arr[i]);
    //printf("first array of even numbers %d\n",arr[i]);
        if (arr[i] % 2 == 0) {
            even[eIndex++] = arr[i];
        } else {
            odd[oIndex++] = arr[i];
        }
    }
    printf("After array is Arranges:\n");
    // Print even numbers in ascending order
    for (int i = 0; i < eIndex; i++) {
        printf("%d ", even[i]);
    }
    // Print odd numbers in descending order
    for (int i = oIndex - 1; i >= 0; i--) {
        printf(" %d ", odd[i]);
    }
    printf("\n");
    return 0;
}

