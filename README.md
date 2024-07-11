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
