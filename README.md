#include <iostream>
using namespace std;

int main() {
    int num, reversed = 0;

    cout << "Enter a number: ";
    cin >> num;

    int original = num;  // store for display

    while (num != 0) {
        int digit = num % 10;          // get last digit
        reversed = reversed * 10 + digit; // add digit to reversed number
        num = num / 10;                // remove last digit
    }

    cout << "Original number: " << original << endl;
    cout << "Reversed number: " << reversed << endl;

    return 0;
}
