using namespace std;
#include<iostream>
#include<math.h>
int main() {
   float a, b, c, area, s;
   cout<<"enter the three sides of the triangle: ";
   cin>>a>>b>>c;

   s= (a+b+c)/2;

   area= sqrt(s*(s-a)*(s-b)*(s-c));

   cout<<"area= "<<area;

   return 0;
}
