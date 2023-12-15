#include <iostream>
using namespace std;
double add (double a,double b);
double subtraction(double a,double b);
double multiplication(double a,double b);
double division (double a,double b);
int main(){
    double add (double a,double b) ;
    double subtraction(double a,double b);
    double multiplication(double a,double b);
    double division (double a,double b);
    double a;
    double b;
    char operation;
    cout<<"Enter the operations(+,-,*,/):";
    cin>>operation;
    cout<<"Enter the first number:";
    cin>>a;
    cout<<"Enter the second number:";
    cin>>b;
    if(operation=='+'){
        cout<<"The result is: "<<add(a,b)<<endl;
    }else if(operation=='-'){
        cout<<"The result is: "<<subtraction(a,b)<<endl;
    }else if(operation=='*'){
        cout<<"The result is: "<<multiplication(a,b)<<endl;
    }else if(operation=='/'){
        cout<<"The result is: "<<division(a,b)<<endl;
    }else{
        cout<<"syntax error";
    }
    return 0;
}
double add (double a,double b){
    return a+b;
}
double subtraction(double a,double b){
    return a-b;
}
double multiplication(double a,double b){
    return a*b;
}
double division (double a,double b){
    if(b==0){
        cout<<"The second number can't be 0.";
        return 0.0;
    }else{return a/b;}
}
