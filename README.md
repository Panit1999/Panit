#include <iostream>
#include <string>
using namespace std;
int main()
{
    float Sum = 0;
    float Grade = 0;
    int round = 0;
  do{
      char GradeStr;
      cout<<"Enter the letter grade (Enter 'X' to exit)";
      cin>>GradeStr;
      if(GradeStr == 'a' || GradeStr == 'A'){Grade += 4;Sum = Sum + 1;}
      else if(GradeStr == 'b' || GradeStr == 'B'){Grade += 3;Sum = Sum + 1;}
      else if(GradeStr == 'c' || GradeStr == 'C'){Grade += 2;Sum = Sum + 1;}
      else if(GradeStr == 'd' || GradeStr == 'D'){Grade += 1;Sum = Sum + 1;}
      else if(GradeStr == 'f' || GradeStr == 'F'){Grade += 0;Sum = Sum + 1;}
      else if(GradeStr == 'x' || GradeStr == 'X')round = 1;
      else cout<<"Plase Enter again!!\n";
    }while(round != 1);
  cout<<"Total Grade Point: "<<Grade<<endl;
  cout<<"GPA :  "<< ((Grade/Sum)*100)/100 << endl;
  return(0);
}
