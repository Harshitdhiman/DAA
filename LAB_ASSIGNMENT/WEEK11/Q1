#include <iostream>
#include <vector>
#include <climits>
using namespace std;

int matrixChainMultiplication(vector<int> &dims, int i, int j)
{
    
    if (j <= i + 1) {
        return 0;
    }
    int min = INT_MAX;
 
    for (int k = i + 1; k <= j - 1; k++)
    {
        
        int cost = matrixChainMultiplication(dims, i, k);
 
        cost += matrixChainMultiplication(dims, k, j);
 
        cost +=    dims[i] * dims[k] * dims[j];
 
        if (cost < min) {
            min = cost;
        }
    }
 
    
    return min;
}
int main()
{
    int n;
    cin>>n;
    vector<int>v(2*n);
    for(int i=0;i<2*n;i++)
    cin>>v[i];
    
    vector<int>dims(n+1);
    int k=0,i=0;
    while(i<v.size())
    {
        if(i==0)
        {
            dims[k++]=v[i];
            i++;
            dims[k++]=v[i];
            i++;
            
        }
        else
        {
            i++;
           dims[k++]=v[i];
            i++;
            
        }
    }
    cout << "The minimum cost is " << matrixChainMultiplication(dims, 0, dims.size()-1);
    return 0;
}
