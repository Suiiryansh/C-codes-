#include <iostream>
#include <cstlib>
#include <ctime>

using namespace std;
int main (){
    srand(time(0));
    int scecretNumber = rand() % 100+1;
    int guess = 0;
    int tries = 0;

    cout<<"--welcome to the guessing game! ---"<<endl;
    cout<<"--i have picked the numebr between 1 and 100 --"<<endl;
    // game loop 
    do{
        cout<< "enter your guess: ";
        cin>> guess;
        tries++;

        if (guess > scecretNumber){
            cout<<"too high! try again."<<endl;
        } else if (guess < scecretNumber){
            cout<<"too low! try again."<<endl;
        } else {
            cout<<"congratulations! you guessed the number in "<< tries <<" tries!"<<endl;
        }
    }
}
