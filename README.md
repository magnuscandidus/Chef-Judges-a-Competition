# Chef-Judges-a-Competition
#include <iostream>
#include<bits/stdc++.h>
using namespace std;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--){
	    int n;
	    cin>>n;
	    int a[n],b[n];
	    int suma=0,sumb=0;
	    for(int i=0;i<n;i++){
	        cin>>a[i];
	        suma=suma+a[i];
	    }
	    sort(a,a+n);
	    suma=suma-a[n-1];
	    for(int i=0;i<n;i++){
	        cin>>b[i];
	        sumb=sumb+b[i];
	    }
	    sort(b,b+n);
	    sumb=sumb-b[n-1];
	    if(suma<sumb){
	        cout<<"Alice"<<endl;
	    }
	    else if(sumb==suma){
	        cout<<"Draw"<<endl;
	    }
	    else{
	        cout<<"Bob"<<endl;
	    }
	}
	return 0;
}
