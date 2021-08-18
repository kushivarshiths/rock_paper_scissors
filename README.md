/*This is a rock paper scissors game */
#include<iostream>
#include<stdlib.h>
int main(){
  int usr = 0;
  
  int computer;

  srand(time(NULL));

  computer = std::rand()%3 + 1;

 std::cout << "======================\n";
 std::cout << "rockpaperscissors\n";
 std::cout << "=======================\n";

 std::cout << "1)✊\n";
 std::cout << "2)✋\n";
 std::cout << "3)✌️\n";

std::cout << "==========================\n";
std::cout << "shooot\n";

std::cin >> usr;

if(usr > 3){
  std::cout << "ERROR: WRONG INPUT\n";
  }

std::cout << "===============================\n";

if(usr == 1 && computer == 3){
  std::cout << "You Win!\n";
  std::cout <<"========================\n";
}
else if(usr == 2 && computer == 1){
  std::cout << "You Win!\n";
  std::cout <<"========================\n";
  }
  else if(usr == 3 && computer == 2){
    std::cout << "You Win!\n";
    std::cout <<"========================\n";
}
else if(usr == computer){
    std::cout << "It's a Draw!\n";
    std::cout <<"=======================\n";
}  
else{
  std::cout << "You Lose!\n";
  std::cout << computer <<"\n";
  std::cout <<"=======================\n";

}

}
