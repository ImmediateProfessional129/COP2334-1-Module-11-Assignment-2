# COP2334-1-Module-11-Assignment-2
This is a repository link of the COP2334-1 Module 11 Assignment 2

// This program is designed to transcribe a high school student's name, age, and GPA.

// Include the iostream library
#include <iostream>
#include <string> // Include the string library
using namespace std; // Use the standard namespace

class Student { // Define a class called Student
private: // Declare private members
    string name_of_student; // Declare a string variable to store the name of the student.
    int age_of_student; // Declare an integer variable to store the age of the student.
    char grade_letter; // Declare a character variable to store the grade letter of the student.
public: // Declare public members
    // Constructor
    Student(string name, int age, char grade) { // Define a constructor that takes three parameters: name, age, and grade.
        name_of_student = name; // Set the name of the student to the value of the name parameter.
        age_of_student = age; // Set the age of the student to the value of the age parameter.
        grade_letter = grade; // Set the grade letter of the student to the value of the grade parameter.
    }
    // Setter methods
    void set_name(string name) { // Define a method called set_name that takes a string parameter and sets the name of the student.
        name_of_student = name; // Set the name of the student to the value of the name parameter.
    }
    void set_age(int age) { // Define a method called set_age that takes an integer parameter and sets the age of the student.
        age_of_student = age; // Set the age of the student to the value of the age parameter.
    }
    void set_grade(char grade) { // Define a method called set_grade that takes a character parameter and sets the grade letter of the student.
        grade_letter = grade; // Set the grade letter of the student to the value of the grade parameter.
    }
    // Getter methods
    string get_name() { // Define a method called get_name that returns the name of the student.
        return name_of_student; // Return the name of the student.
    }
    int get_age() { // Define a method called get_age that returns the age of the student.
        return age_of_student; // Return the age of the student.
    }
    char get_grade() { // Define a method called get_grade that returns the grade letter of the student.
        return grade_letter; // Return the grade letter of the student.
    }
    // Display method
    void display() { // Define a method called display that displays the name, age, and grade letter of the student.
        cout << "Student 1:" << endl; // Display a message indicating that the student information is being displayed.
        cout << "Name: " << name_of_student << endl; // Display the name of the student.
        cout << "Age: " << age_of_student << endl; // Display the age of the student.
        cout << "Grade: " << grade_letter << endl; // Display the grade letter of the student.
    }
}; // End of the Student class

int main() { // Define the main function
    // Instantiate two Student objects
    Student student1("Emily", 19, 'B'); // Create a Student object called student1 with the name "Emily", age 19, and grade 'B'.
    Student student2("Ryan", 21, 'A'); // Create a Student object called student2 with the name "Ryan", age 21, and grade 'A'.
    // Use the setter methods to assign values to one object
    student1.set_name("Emily"); // Set the name of student1 to "Emily".
    student1.set_age(19); // Set the age of student1 to 19.
    student1.set_grade('B'); // Set the grade letter of student1 to 'B'.
    // Use the constructor to initialize the other object
    student2.set_name("Ryan"); // Set the name of student2 to "Ryan".
    student2.set_age(21); // Set the age of student2 to 21.
    student2.set_grade('A'); // Set the grade letter of student2 to 'A'.
    // Display details for both objects using the display method
    student1.display(); // Display the details for student1.
    student2.display(); // Display the details for student2.
    return 0; // Return 0 to indicate successful program execution.
} // End of the main function
