# Bubble-Sort-
This is the c code for a bubble sort

#include <stdio.h>
 int main (){
   int a[10];
   int size;
   int i;
   int j;
   int temp;
   /*Enter the size of your array*/
   printf("Enter the size of your array:\n");
   scanf("%d", &size);
   
   /*Enter the elements of the array*/
   printf("Enter the elements of your array:\n");
   for(i=0; i<size; i++){
    scanf("%d", &a[i]);
   }
   
   /*Print the unsorted array*/
   for(i=0; i<size; i++){
     printf("%d\t", a[i]);
   }
   
   printf("\n");
   
   for(i=0; i<size; i++){
     for(j=0; j<size-1; j++){
       if (a[j]>a[j+1]) {
         temp = a[j];
         a[j] = a[j+1];
         a[j+1] = temp;
       }
     }
   }
   /*Print the sorted array*/
   for(i=0; i<size; i++){
     printf("%d\t", a[i]);
   } 
   
 }
