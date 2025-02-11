# -Police-Recruits
#include<iostream>
using namespace std;
int main(){
    int n, c=0,p=0, count=0;
   cin>>n;
   int arr[n];
   for(int i=0;i<n;i++){
       cin>>arr[i];
   }
   for(int i=0; i<n; i++){
       if(arr[i]==-1){
           if(p>0){
               p--;
           }
           else{
               count++;
           }
       }
       else{
           p+=arr[i];
       }
      
   }
   cout<<count;
}
