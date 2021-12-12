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


















     
