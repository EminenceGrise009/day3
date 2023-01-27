# day3
// #include<iostream>
#include<bits/stdc++.h>

using namespace std;

// 1. same name
// 2. either diff. num of parameters 
    //  diff. type of parameters

int maxi(int n1,int n2){
  if(n1>n2)return n1;
  return n2;
}

int maxi(int n1,int n2,int n3){
  if(n1>n2){
    if(n1 > n3)return n1;
    return n3;
  }else{
    if(n2 > n3)return n2;
    return n3;
  }
}

int maxi(int n1,int n2,int n3,int n4){
  // int a = maxi(n1,n2);
  // int b = maxi(n3,n4);
  // return maxi(a,b);

  int a = maxi(n1,n2,n3);
  return maxi(a,n4);
}

int main(){

// max()
  cout<<maxi(2,5);
  cout<<maxi(2,5,3);
  cout<<maxi(2,5,3,5);


  return 0;
}
    
    
    // #include<iostream>
#include<bits/stdc++.h>

using namespace std;

// pass by val.
// void increment(int a){
//   a++;
//   return ;
// }

// pass by pointer
// void increment(int*a){
//   (*a)++;
//   return ;
// }

// pass by ref.
void increment(int&a){
  // (*a)++;
 
//  int&b = 
  a++;
  return ;
}

// ->Address;
// int i ;
// cout<< &i

// int&j =  

int main(){

  int i = 11;
  // int &j = i ;
  // j++;

  // cout<<i<<endl;


  increment(i);

  cout<<i<<endl;

  return 0;
}
    
    
    // #include<iostream>
#include<bits/stdc++.h>

using namespace std;

// itrative fun
// int power(int base,int pow){

//   int num = 1;
//   for(int i = 0;i<pow;i++){
//     num*=base; //num = num*base;
//   }

//   return num;
// }

// void fun(vector<vector<int>>&arr)

void fun(int arr[][]){
  return;
}


// recursive fun
int power(int base,int pow){

  // 1. base case 
  // 2. assumption 
  // 3. cal.

  if(pow == 0)return 1;

  int smlAns = power(base,pow-1); // smlAns - > 2^2
  
  return smlAns*base;
}

int main(){
  int arr[5][4];
  fun(arr);
  cout<<power(2,3);

  return 0;
}
    
    
    
    // #include<iostream>
#include<bits/stdc++.h>

using namespace std;

// int sum(int a,int b);

int sum(int a ,int b= 0){
  return a+b;
}

int main(){

  cout<<sum(2);

  return 0;
}

//  int sum(int a,int b){
//   return a+b;
// }
