#include<stdio.h>
void search(int up,int lw,int key,int arr[]);
int c=0;
int main(){
int up,lw,arr[10],n,i,key;
scanf("%d",&n);
up=n-1;
lw=0;
   for( i=0;i<n;i++){
            scanf("%d",&arr[i]);
        }
        printf("Enter key :");
        scanf("%d",&key);
        search(up,lw,key,arr);
}
void search(int up,int lw,int key,int arr[]){
     int mid=(up+lw)/2;
     c++;
     if(arr[mid]>key){
               up=mid-1;
                  search(up,lw,key,arr);
}
    else if(arr[mid]<key){
               lw=mid+1;
                  search(up,lw,key,arr);
}
else{
     printf("Element found!!\nComparisions %d",c);
}

}
