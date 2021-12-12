# Lecture-15-Intro-to-functions


Declaring and Defining

    #include <iostream>
    using namespace std;

    void welcome();

    int main(){
            welcome();
            return 0;

        }
        void welcome(){

            cout << "Welcome to BSU" << endl;
        }
    

You say hello, I say goodbye
  
    #include <iostream>
    using namespace std;
    void welcome();
    void end();

    void welcome() {

        cout << "Welcome to my program" << endl;
    }

    int main(){
            welcome();
            end();
            return 0;
        }

    void end() {

        cout << "End of program" << endl;
    }

Passing Values - MyCalculation

    #include <iostream>
    using namespace std;

    void myCalculation(int num) {
            num *= 2;
            num += 8;
            cout << num << endl;
        }

    int main()
    {
        int userNum;
        cout << "Enter A Number: ";
        cin >> userNum;
        myCalculation(userNum);

        return 0;
    }



Returning Values - MyCalculation

    #include <iostream>
    using namespace std;

    int myCalculation(int num) {
            num *= 2;
            num += 8;
            return num;
        }

    int main()
    {
        int userNum;
        cout << "Enter A Number: ";
        cin >> userNum;
        userNum = myCalculation(userNum);
        myCalculation(userNum);
        cout << userNum << endl;
        return 0;
    }

Returning Values - Purchase Products

    #include <iostream>
    using namespace std;

    double sumItems(double item1, double item2) {
        double total = item1 + item2;
        return total;
    }
    int main()
    {
        double myMoney = 40.00;
        double shoes = 25.99;
        double tshirt = 11.50;

        if (sumItems(shoes, tshirt) <= myMoney) {
            cout << "you can afford these items" << endl;
        } else {
            cout << "keep saving up" << endl;
        }
    }


Returning Values - Time

#include <iostream>
using namespace std;

string greetings(int time){
    if (time < 12) {
        return "Good Morning";
    }
    else {
        return "Good Afternoon";
    }
}
int main()
{
    cout << "What time is it?" << endl;
    int userInput;
    cin >> userInput;
    cout << greetings(userInput) << endl;
    return 0;
}













     
