#include <iostream>
#include <vector>
#include <string>
#include <fstream>
#include <algorithm>

struct Student {
    std::string firstName;
    std::string surname;
    std::string gender;
    int age;
    int group;
    std::string sport;
    std::vector<std::string> clubs;
};

struct Activity {
    std::string name;
    int maxCapacity;
    int currentCapacity;
    int maleCount;
    int femaleCount;
};
std::vector<Student> students;
std::vector<Activity> sports = {{"Rugby", 20, 0, 0, 0}, {"Athletics", 20, 0, 0, 0}, {"Swimming", 20, 0, 0, 0}, {"Soccer", 20, 0, 0, 0}};
std::vector<Activity> clubs = {{"Journalism Club", 60, 0, 0, 0}, {"Red Cross Society", 60, 0, 0, 0}, {"AISEC", 60, 0, 0, 0}, {"Business Club", 60, 0, 0, 0}, {"Computer Science Club", 60, 0, 0, 0}};

void addStudent();
void viewStudents();
void viewClubs();
void viewSports();
void viewGroupedStudents();
void saveAllFiles();
bool canJoinActivity(Activity& activity, const std::string& gender, bool isSport);

