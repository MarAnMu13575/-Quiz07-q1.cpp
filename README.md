# -Quiz07-q1.cpp

#include iostream>
using namespace std;


long fibonacci (long n){

  long z0 = 0, z1 = 1, k = 0;
  
  if ( n == 1)
  
  k = 1;
  
  for (int i=0; i<n-1; i++){
  
  
  k = z0 + z1;
  
  z0 = z1;
  
  z1 = k;
  
  }
  return k;
  
  
}

long n;


int main(){

  cout<<"Give me a number for fibonacci series:   "<<endl;
  cin >> n;
  
  cout <<"The number in fibonacci series is: "<<endl;
  
  cout<< fibonacci (n);
  

  return 0;
}
