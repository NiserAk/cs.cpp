# cs.cpp
#include<iostream>
using namespace std;
int main()
{
  char prop[1000];int ar[100];
  int i=0,n,a=0;
  clause c;int j=0;
  cout<<"Enter the formula : ";
  while(prop[i-1]!='*') 
  {
    cin>>prop[i];
    i++;
  }
  n=i-2;
  for(int k=0;k<=n;k++)
  {
    cout<<prop[k];
  }
  for(int k=0;k<=n;k++)
  {
    if(prop[k]=='&')
    {
      a=a+1;
      ar[j]=k;
      j++;
    }
  }
  cout<<endl<<a<<endl;
  for(int k=0;k<j;k++)
   {cout<<ar[k]<<endl;} 
     return 0;
}
  
