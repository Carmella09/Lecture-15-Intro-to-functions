# Lecture-15-Intro-to-functions

//EXERCISES PART 1


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


Returning Values - Purchase Products (Declaring)

    #include <iostream>
    using namespace std;

    double sumItems(double item1, double item2) {
        double total = item1 + item2;
        return total;
    }
    int main()
    {
        double myMoney = 40.00;
        double shoes;
        double tshirt;

        cout << "\nHow much is the shoes? ";
        cin >> shoes;

        cout << "\nHow much is the tshirt? ";
        cin >> tshirt;


        if (sumItems(shoes, tshirt) <= myMoney) {
            cout << "\nyou can afford these items" << endl;
        }
        else {
            cout << "\nkeep saving up" << endl;
        }
    }

                                          
                                          
//EXERCISE PART 2 

Time
Write a code that does the following:
1. take time as an input from the user
2. Sends the time to a string function (that takes integer as an argument) and returns the string output, according to the time
3. According to the timings, the following string value should be return to the main function:
1. 0-11 (Good morning)
2. 12-17 (Good afternoon)
3. 18-21 (Good Evening)
4. 22-24 (Good night)

        #include <iostream>
        using namespace std;

        string greetings(int time) {
            if (time >= 0 && time <= 11) {
                return "Good Morning";
            }
            else if (time >= 12 && time <= 17) {
                return "Good Afternoon";
            }
            else if (time >= 18 && time <= 21) {
                return "Good Evening";
            }
            else if (time >= 22 && time <= 24) {
                return "Good Night";
            }
            else {
                return "Invalid Input";
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

    
Root Value
Write a code that does the following:
1. The main function takes an integer input from the user
2. Then create another function that receives that integer input and calculate the root value from 1-10 for that number
3. The function will then send back a message to the main function that states that the code is completed

        #include <iostream>
        #include <string>
        #include <math.h>
        #include <cmath>
        using namespace std;

        string message(double num)
        {

            cout << "\nOutput:: " << endl;
            double y = 1;
            do
            {
                cout << y << " Root Value of " << num << " is: ";
                double x = 1 / y;
                double r = pow(num, x);
                cout << r << endl;
                y++;
            } while (y != 11);

            return "\nEND";
        }

        int main()
        {

            int num, fact = 1;

            cout << "Enter a number you want to find the root value of: ";
            cin >> num;

            while (cin.fail())
            {
                cout << "Invalid Input : " << endl;
                cout << "Enter the Number again: ";
                cin.clear();
                cin.ignore(1000, '\n');
                cin >> num;
            }
            cout << message(num) << endl;

            return 0;

        }

Exponent Value
Write a code that does the following:
1. The main function takes an integer input from the user
2. Then create another function that receives that integer input and calculate the exponent value from 1-10 for that number
3. The function will then send back a message to the main function that states that the code is completed

        #include <iostream>
        #include <string>
        #include <math.h>
        #include <cmath>
        using namespace std;

        string message(double num)
        {

            cout << "\nOutput:: " << endl;
            double y = 1;
            do
            {
                cout << y << " Exponent Value of " << num << " is: ";
                cout << pow(num, y) << endl;
                y++;
            } while (y != 11);

            return "\nEND";
        }

        int main()
        {

            int num, fact = 1;

            cout << "Enter a number you want to find the exponent value of: ";
            cin >> num;

            while (cin.fail())
            {
                cout << "Invalid Input : " << endl;
                cout << "Enter the Number again: ";
                cin.clear();
                cin.ignore(1000, '\n');
                cin >> num;
            }
            cout << message(num) << endl;

            return 0;

        }


//NOT EXERCISE

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
    







     
