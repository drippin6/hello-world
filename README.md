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
int main() {
    int choice;
    do {
        std::cout << "Menu:\n";
        std::cout << "1. Add Student\n";
        std::cout << "2. View Students (ALL and per group)\n";
        std::cout << "3. View Clubs/ Societies\n";
        std::cout << "4. View Sports\n";
        std::cout << "5. View Grouped Students\n";
        std::cout << "6. Save all Files\n";
        std::cout << "7. Exit\n";
        std::cout << "Enter your choice: ";
        std::cin >> choice;

        switch (choice) {
            case 1:
                addStudent();
                break;
            case 2:
                viewStudents();
                break;
            case 3:
                viewClubs();
                break;
            case 4:
                viewSports();                break;
            case 5:
                viewGroupedStudents();
                break;
            case 6:
                saveAllFiles();
                break;
            case 7:
                std::cout << "Exiting...\n";
                               break;
            default:
                std::cout << "Invalid choice! Please try again.\n";
        }
    } while (choice != 7);

    return 0;
}

