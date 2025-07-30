# find-smallest-no.-and-its-index-in-given-array.c
// C program to find smallest no. and its index in given array elements
#include <stdio.h>

int main() {
    int s,sm,i,n;

    printf("Enter the size of the array: ");
    scanf("%d", &s);

    int a[s]; 
    printf("Enter elements:\n");
    
    for (int i=0;i<s;i++)
        scanf("%d", &a[i]);
        
        sm=a[0];
    for (int i = 1; i <s; i++){
        if(sm>a[i]){
        sm=a[i];
         n=i;
        }
    }
    printf("index=%d",n);
    printf("smallest no.=%d",sm);
    return 0;
}
