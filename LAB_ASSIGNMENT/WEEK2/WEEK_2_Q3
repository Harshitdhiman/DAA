#include<stdio.h>
#include <stdlib.h>


int main()
{
    int t;
    scanf("%d", &t);

    while(t){
        int n;
        scanf("%d", &n);

        int arr[n];
        for(int i=0;i<n;i++)
            scanf("%d", &arr[i]);

        int k,count=0;
        scanf("%d", &k);

        for(int i=0;i<n;i++){
            for(int j=1; j<n; j++)
                if(arr[j]-arr[i]==k)
                    {
                        count++;
                    }
        }
        printf("%d pairs found", count);

        t--;
    }
}
