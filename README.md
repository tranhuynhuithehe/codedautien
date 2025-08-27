#include<iostream>
using namespace std;
using ll = long long;

bool check(ll n){
  int tong=0;
  while(n!=0){
    tong += (n%10);
    n/=10;
  }
  if((tong%10)%8==0 )
    return true;
  else return false;
}
int main(){
  ll n;
  cin>>n;
  if(check(n)== true)
    cout<<"yes\n";
  else cout<<"no\n";  
  return 0;
}
