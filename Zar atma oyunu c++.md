//Zar atma oyunu

#include <iostream>
#include <stdlib.h>
#include <time.h>
#include <cmath>
using namespace std;
int main () {
    int a,b,c,n,toplam1,toplam2;
    srand(time(NULL));
    cout << "kaç tane zar atmak istiyon zımbo : ";
    cin >> n;
    toplam2 = 0;
    toplam1 = 0;
    if (n<=0){
        cout << "mal mısın amk?";
    }
    else {
        for (int i = 0 ; i<n ; i++){
        a = rand () % 6+1;
        b = rand () % 6+1;
        toplam1 += a;
        toplam2 += b;
        }
        if (toplam1<toplam2){
            cout << "oyuncu " << toplam1 << " skoru ile, " << toplam2 << " skorlu yapay zekaya yenildi";
        }
        else if (toplam1==toplam2){
            cout << toplam1 << " skoru ile oyuncu ve yapay zeka berabere";
        }
        else {
            cout << "oyuncu " << toplam1 << " skoru ile " << toplam2 << " skorlu yapay zekayı yendi";
        }
    }
}



