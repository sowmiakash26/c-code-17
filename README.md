#include<stdio.h>
void sort(int arr[],int n){
int temp;
for(int i=0;i<n-1;i++){
    for(int j=i+1;j<n;j++){
        if(arr[i]>arr[j]){
            temp=arr[i];
            arr[i]=arr[j];
            arr[j]=temp;
        }
    }
}
for(int i=0;i<n/2;i++){
    printf("%d ",arr[i]);
    }
for(int j=n-1;j>=n/2;j--){
    printf("%d ",arr[j]);
}
return;
}

int main()
{
    int arr[]={11,22,44,16,88,77,55};
    int n=sizeof(arr)/sizeof(arr[0]);
    sort(arr,n);
    return 0;
}
