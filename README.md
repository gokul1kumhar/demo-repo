#include<iostream.h>
#include<conio.h>
using namespace std;
class b; class a{
int m;
public:
void input() {
cout<<"enter first number: ";
cin>>m;
}
friend void max(a, b);
};
class b{
int n;
public:
void getdata() {
cout<<"enter second number: ";
cin>>n;
}
friend void max(a, b);
};
void max(a l1, b l2) {
if(l1.m > l2.n) {
cout<<"max= "<<l1.m;
}
else {
cout<<"max= "<<l2.n;
}
}
void main() {
a l1; b l2;
l1.input();
l2.getdata();
max(l1, l2);
getch();
}
