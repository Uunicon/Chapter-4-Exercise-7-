# Chapter-4-Exercise-7-

// instr2.cpp -- reading more than one word with getline


#include <iostream>
#include <string>
using namespace std;
	
struct Pizza 
{
	char str1[20];
	float dia;
	float weg;
};
int main()

{
    Pizza *p=new Pizza ;
    cout<<"Please enter each of information:"<<endl;
    cin.getline(p->str1,20);                                //reading more than one word with getline
    cin>>p->dia>>p->weg;
    cout<<p->str1<<" "<<(*p).dia<<" "<<p->weg<<endl;        //different ways to cout 
    return 0; 
}
