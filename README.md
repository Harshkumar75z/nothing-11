// Calculate the product of all the elements in the given array.
#include <iostream>
using namespace std;
int main()
{
    int Product=1;
    int n;
    cout<<"Enter Elements : ";
    cin>>n;
    int arr[n];
    for(int i=0;i<=n-1;i++){
        cin>>arr[i];
    }
    for(int i=0;i<=n-1;i++){
        Product = Product*arr[i];
    }
    cout<<Product;
}


// Find the second largest element in the given Array in one pass.
#include <iostream>
#include <climits>
using namespace std;
int main()
{
    int arr[]={1,3,5,7,9};
    int n=sizeof(arr)/4;
    int max=INT_MIN;
    int smax=INT_MIN;
    for(int i=0;i<n;i++){
        if(arr[i]>max){
            smax=max;
            max=arr[i];
        }
    }
    cout<<max<<endl;
    if(smax==INT_MIN)
    cout<<"No Second largest exist";
    else cout<<smax<<endl;

}

// Find the minimum value out of all elements in the array.
#include<iostream>
using namespace std;
int main()
{
    int n;
    cout<<"Enter the number of element in array : ";
    cin>>n;
    int arr[n];
    for(int i=0;i<=n-1;i++){
        cin>>arr[i];
    }
    int min=arr[0];
    for(int i=1;i<=n-1;i++){
        if(min>arr[i]) min=arr[i];
    }
    cout<<"Minimum Element is ";
    cout<<min;
}

