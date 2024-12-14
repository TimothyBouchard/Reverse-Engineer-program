#include <iostream>

using namespace std;

int displayMenu() {
    cout << "----------" << endl;
    cout << "- 1). Add-" << endl;
    cout << "- 2). Subtract-" << endl;
    cout << "- 3). Multiply-" << endl;
    cout << "- 4). Exit -" << endl;
    cout << "----------" << endl;

    return 0;
}
int checkInput() {  // implemented a input check function to make sure the inputs are only numbers
                    // having a user input without any validations can open the system up to 
                    // un-trusted data inputs. 
    int input;
    while (!(cin >> input)) {
        cout << "Invalid input" << endl;
        cin.clear(); 
        cin.ignore(numeric_limits<streamsize>::max(), '\n'); // ignore all non-number charactors 
    }
    return input;
}
 
int main() {
    int userinput = 0;
    int num1, num2;
    char equals = '=';

    while (userinput != 4) { 
        displayMenu();
        //cin >> userinput; // accepting untrusted data without any checks. 
        userinput = checkInput();

        if (userinput == 1) {
            cout << "- 1)Add -" << endl;
                //cin >> num1 >> num2; // no secerity checks to make sure only numbers are entered. 
            num1 = checkInput();
            num2 = checkInput();
            cout << equals << num1 + num2 << endl; // processing untrusted data 
        }
        if (userinput == 2) {
            cout << "- 2)Subtract -" << endl;
               // cin >> num1 >> num2; // accepting untrusted data
            num1 = checkInput();
            num2 = checkInput();
            cout << equals << num1 - num2 << endl; // processing unrusted data
        }
        if (userinput == 3) {
            cout << "- 3)Multiply -" << endl;
               // cin >> num1 >> num2; //accepting untrusted data
            num1 = checkInput();
            num2 = checkInput();
            cout << equals << num1 * num2 << endl; // processing the data 
        }
        if (userinput == 4) {
            cout << "-Exit-" << endl;
        }
    }
}
