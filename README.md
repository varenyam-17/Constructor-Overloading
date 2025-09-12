# Constructor-Overloading
---------------------------------------------
       C++ PROGRAM: Constructor Overloading
---------------------------------------------

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
------
