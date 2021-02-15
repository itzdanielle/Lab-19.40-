# Lab-19.40-
#include <iostream>
using namespace std;

void input (int& meter) {
cout << "Please input how many meters you would like to convert" << endl;
cin >> meter;
}
double calculations2 ( int& meter, double& foot){
  double dfoot = meter /0.3048; 
  foot = int (dfoot);
  double inches = (dfoot - foot)* 12;
  return inches;
}
void results2 (double inches, double foot, int meter) { 
 cout << "Inches : " << inches << endl;
 cout << "Feet : " << foot << endl;
 cout << "Meters : " << meter << endl;
}


int main() {
  double inches;
  double foot;
  int meter;
  input (meter);
  inches = calculations2 (meter, foot);
  results2 (inches, foot, meter);
}
