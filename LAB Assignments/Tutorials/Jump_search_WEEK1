#include<iostream>
#include<math.h>
using namespace std;
int JumpSearch(int A[],int key,int n)
{
    int m=sqrt(n);
    int i=0;
    while(A[m]<=key && m<n)
    {
        i=m;
        m=m+sqrt(n);
        if(m>n-1)
            m=n;
    }
    for(int k=i;k<m;k++)
    {
        if(A[k]==key)
            return k;
    }
    return -1;
}
int main()
{
    int n,key;
     cout<<"enter the size of array:";
     cin>>n;
     
    int A[n];
    cout<<"enter the elements:";
    for(int i=0;i<n;i++)
        cin>>A[i];
        
     cout<<"enter the key:";
     cin>>key;
     
     int c= JumpSearch(A,key,n);
     if(c>0)
        cout<<"found";
     else
        cout<<"not found";
    return 0;
}
