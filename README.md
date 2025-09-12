# Constructor-Overloading


AIM:
----
To write a C++ program that demonstrates constructor overloading.

THEORY:
-------
- Constructor is a special member function in C++ that is automatically called 
  when an object is created.
- Constructors initialize the data members of a class.
- Constructor overloading means having more than one constructor in a class 
  with different parameter lists.
- This allows objects to be initialized in multiple ways.

SYNTAX:
-------
class ClassName {
    public:
        ClassName();                  // Default constructor
        ClassName(int a);             // Parameterized constructor
        ClassName(int a, int b);      // Another parameterized constructor
};

When objects are created, the appropriate constructor is chosen based on 
the arguments passed.

PROGRAM:
--------
#include <iostream>
using namespace std;

class Rectangle {
    int length, breadth;

public:
    // Default constructor
    Rectangle() {
        length = 0;
        breadth = 0;
    }

    // Constructor with one parameter
    Rectangle(int l) {
        length = l;
        breadth = l; // Square
    }

    // Constructor with two parameters
    Rectangle(int l, int b) {
        length = l;
        breadth = b;
    }

    int area() {
        return length * breadth;
    }

    void display() {
        cout << "Length = " << length 
             << ", Breadth = " << breadth 
             << ", Area = " << area() << endl;
    }
};

int main() {
    Rectangle r1;             // Calls default constructor
    Rectangle r2(5);          // Calls constructor with one parameter
    Rectangle r3(4, 6);       // Calls constructor with two parameters

    r1.display();
    r2.display();
    r3.display();

    return 0;
}

OUTPUT:
-------
Length = 0, Breadth = 0, Area = 0
Length = 5, Breadth = 5, Area = 25
Length = 4, Breadth = 6, Area = 24

CONCLUSION:
-----------
Constructor overloading allows creating multiple constructors in a class
to initialize objects in different ways. It improves flexibility and 
readability of code.

