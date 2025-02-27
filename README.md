Download link :https://programming.engineering/product/name-lab-solution/

# Name-Lab-Solution
Name Lab Solution
Introduction:

The objective of this lab is to create a vector of Name objects that are initialized from a file.
In addition, the object will be broken into a pair of files.

Instructions:

Create a class called Name which will be used by the main program, called NameDriver.cpp.

Separate the code into 2 files:

Name.h contains the declaration. Please add ‘guardrails’ to your .h file

Name.cpp contains the implementation. Name.cpp has a #include “Name.h”


Each Name object contains a first and last name.

Declare all the methods and constructors (getters, setters, default constructors) in Name.h

Define and implement the methods in the Name.cpp file.

In Name.h


Declare private data members for the class, a first name (fname) and a last name (lname). Do not worry about a middle name or initial.

Declare public members getFirstName, getLastName, printName (prints firstName <space> lastName, a default constructor and a constructor that takes a string.

Add guards to this file

#ifndef NAME_H

#define NAME_H

…. Class definition goes here

#endif

In Name.cpp

In the empty default constructor, initialize the fname and lname to “First” and “Last” respectively.

Create a constructor that will initialize both fname and lname from a string (a full line) which will have to be parsed.

For now, assume no middle name.

Hint: Using find and substr, find the index of the comma, and split the long string into fname and lname.

Define the setters, getters, and helper functions for this class as declared in the .h file.

In NameDriver.cpp (main)

Open a file called NamesLastFirst.txt (actually has comma separated values)

Read each line and pass it to the Name constructor that takes a string.

Create a name object for each and append it to a vector of name objects.

Print the vector in reverse order: firstname lastname

Extra Credit: Create the vector of pointers to Name objects.

Compile the code with:

g++ Name.cpp NameDriver.cpp -o name

Run the code with:

./name

File contents (NamesLastFirst.csv):

Cyrus,Miley

Gaga,Lady

Grande,Ariana

Keys,Alicia

Mars,Bruno

Sheeran,Ed

Stiles,Harry

Swift,Taylor

Example Output:

Taylor Swift

Harry Stiles

Ed Sheeran

Bruno Mars

Alicia Keys

Ariana Grande

Lady Gaga

Miley Cyrus
