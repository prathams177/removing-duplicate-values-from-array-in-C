# removing-duplicate-values-from-array-in-C


#include <stdio.h>

int main()
{
    int arr[10]={1,2,5,7,1,7,3,9,2,5};
    int i,j,k,n=10,temp;
    for(i=0;i<n;i++){
        for(j=i+1;j<n;j++){
            if(arr[i]==arr[j]){
                for(k=j;k<n;k++){
                    arr[k]=arr[k+1];
                }
                n--;
                j--;
                
            }
            
        }
        
    }
    
    for(i=0;i<n;i++)
    printf("%d",arr[i]);

    return 0;
}
