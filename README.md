# hello-world 1st Beckham's project
//program to compute co curricular activities for new students
#include <iostream>
#include <string>
using namespace std;
int main()
{

//structure used to represent a student
  struct student{ 
  string name;
  char gender;//'m' is for male and 'f' is for female
  bool participatinginsport;
  int clubs;
}
//constants for maximum capacity
    const int max club capacity=60;
    const int max sport capacity=20;
    const int num students=50*3//total number of students
//function to validate gender constraints 
    bool validgenderratio(int males,int females,double ratio)
{
  double totalstudents=males+females;
  double maleratio=males/totalstudents;
  double femaleratio=females/totalstuents;
  return (maleratio<=maxratio)&&(femaleratio<=maxratio);
}  
  
  
