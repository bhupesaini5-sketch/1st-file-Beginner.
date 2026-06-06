#include <iostream>
using namespace std;
int main (){
    int a;
    cout <<"Enter a no. : ";
    cin >>a;
    if (a%2!=0) {
        int n=a/2+1;
        for (int i=1;i<=n;i++) {
            for (int j=1; j<=n-i+1;j++) {
                cout <<"  ";
            }
            for (int j=1; j<=i;j++) {
                cout <<"* ";
            }
            for (int j=1; j<=i-1;j++) {// star
                cout <<"* ";
            }
            cout <<endl;
        }
        for (int i=2;i<=n;i++) {
            for (int j=1; j<=i;j++) {
                cout <<"  ";
            }
            for (int j=1; j<=n-i+1;j++) {
                cout <<"* ";
            }
            for (int j=1; j<=n-i;j++) {// star
                cout <<"* ";
            }
            cout <<endl;
        }
    }
    else {
        int n=a/2;
        for (int i=1;i<=n;i++) {
            for (int j=1; j<=n-i+1;j++) {
                cout <<"  ";
            }
            for (int j=1; j<=i;j++) {
                cout <<"* ";
            }
            for (int j=1; j<=i;j++) {// star
                cout <<"* ";
            }
            cout <<endl;
        }
        for (int i=1;i<=n;i++) {
            for (int j=1; j<=i;j++) {
                cout <<"  ";
            }
            for (int j=1; j<=n-i+1;j++) {
                cout <<"* ";
            }
            for (int j=1; j<=n-i+1;j++) {// star
                cout <<"* ";
            }
            cout <<endl;
        }
    }
}
