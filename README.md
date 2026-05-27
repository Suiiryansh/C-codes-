This file contains the code for The guessing game in c++ 
USED:-    
    1.IOstream- input output stream 
    2. CSTLIB
    3. CTIME 
in this game you can guess the numbers between 1 and 100 OR you can edit and change it to any , then if your guess is low it pop up a message that the number is too low and if the number is high it will pop up the number is too high 
The game end when the number is perfect!

enjoy playing the guessing game!!
END 


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
