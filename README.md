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























     
