#include <iostream>

using namespace std;

int main()
{
    int n;
    cin>>n;
    int i=2;
    if(n==0) {
        cout<<0;
    }
    else {
    int r1=1;
    int r0=0;
    while(i<=n) {
        int x=r1;
        r1=r0+r1;
        r0=x;
        i++;
    }
    cout<<r1;
}
}
