#include <iostream>
#include <cstdlib>
#include <ctime>
#include <wchar.h>
#include <Windows.h>
#include <algorithm>
#include <vector>
#include <string>
#include <conio.h>


using namespace std;



int main()
{
    long x, y;
    char dir;
    cout << "Enter X: ";
    cin >> x;
    while (true) {
            cout << "\n\nEnter Y: ";
            cin >> y;
            cout << "Enter 1   x + y\n";
            cout << "Enter 2   x - y\n";
            cout << "Enter 3   x / y\n";
            cout << "Enter 4   x * y\n";
            cin >> dir;
        while (dir != '\r') {
            switch (dir) {
            case '1':cout << "Resualt: " << x + y;
                x = x + y;break;break;
            case '2':cout << "Resualt: " << x - y;
                x = x - y;break;break;
            case '3':cout << "Resualt: " << x / y;
                x = x / y;break;break;
            case '4':cout << "Resualt: " << x * y;
                x = x * y;break;break;
            }
            break;
        }
    }


    return 0;
}
