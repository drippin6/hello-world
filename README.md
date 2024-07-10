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
  int totalstudents=males+females;
  double maleratio=males/totalstudents;
  double femaleratio=females/totalstuents;
  return (maleratio<=maxratio)&&(femaleratio<=maxratio);
}  
//validate total number of clubs and sports
  if(clubs>3){
  cout<<"Error:maximum of 3 clubs allowed"<<end1;\n;
  return 1;
  }
  if(sports>1){
  cout<<"Error:maximum of 1 sport allowed"<<end1;\n;
  return 1;
  }
//validate capacity for clubs and sports
  if(clubs*max club capacity+sports*max sport capacity>students){
  cout<<"Error:capacity exceeded"<<end1;
  return 1;
  }

//validate gender ratio for clubs and sports
  if
  (validgenderratio(clubs,1,0.5))
  {
  cout<<"Error:Gender ratio exceeded"<<end1;
  return 1;
  }
  clubs++;
  }
  if
  (validgenderratio(sports,1,0.75))
  {
  cout<<"Error:Gender ratio exceeded"<<end1;
  return 1;
  }
  sports++;
  }
  for(int i=0;i<students;i++)
  {
  if 
  (students[i]participatinginsport){

  cout<<"Selected activities"<<end1;
  if(sports>0){
  cout<<"sport"<<end1;
  }
  for(int i=0;i<clubs;i++){
  cout<<"clubs"<<end1;
  }
  system("pause");
  return 0;
  }
  
  
  
  
  
