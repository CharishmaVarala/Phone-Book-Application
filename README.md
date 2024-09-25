# Phone-Book-Application

This is a simple phonebook application written in C++ that allows users to:

Display all names and phone numbers.
Add new names and phone numbers.
Modify existing phone numbers.
Search for names in the phonebook.
The data is stored in a text file (phonebook.txt), and all modifications are reflected in the file.

Features
Add a Contact: You can add new contacts with names and phone numbers.
Update a Contact: Modify the phone number of an existing contact.
Search for a Contact: Search by name to display the associated phone number.
List All Contacts: Display all contacts with their phone numbers.
Persistent Storage: All data is saved in a file (phonebook.txt) so it can be used between different runs of the application.

Prerequisites
A C++ compiler (e.g., g++).
A terminal or command prompt for running the application.
A text editor or IDE for modifying and compiling the code.
Setup
Clone the repository or download the project files.
Ensure you have a phonebook.txt file in the same directory as the compiled application. This file will store the contact details. If the file does not exist, it will be created upon running the application.
Creating the phonebook.txt file
If you want to create a sample phonebook manually, use the following format:

Copy code
John Doe
123-456-7890
Jane Smith
098-765-4321
Each name is followed by a phone number, and there should be a newline between contacts.

How to Compile and Run
To compile and run the program, follow these steps:

Linux/MacOS:
Open a terminal.
Navigate to the directory where the source code is located.
Compile the program using g++:
bash
Copy code
g++ phonebook.cpp -o phonebook
Run the program:
bash
Copy code
./phonebook
Windows:
Open a command prompt.
Navigate to the directory where the source code is located.
Compile the program using g++:
bash
Copy code
g++ phonebook.cpp -o phonebook.exe
Run the program:
bash
Copy code
phonebook.exe
How to Use
When you run the program, you'll see the following menu:

css
Copy code
A - Add a name and phone number
C - Change a phone number
F - Find a name
L - List all names
Q - Quit
Adding a New Contact:
Choose the option A to add a new name and phone number.
Enter the contact name and phone number when prompted.
Changing a Phone Number:
Choose the option C to change an existing phone number.
Enter the name of the contact whose number you want to change, then provide the new number.
Finding a Contact:
Choose the option F to search for a name.
Enter the name or part of the name you're looking for, and the program will display all matches.
Listing All Contacts:
Choose the option L to list all contacts with their phone numbers.
Exiting the Program:
Choose the option Q to quit the program.
File Structure
bash
Copy code
.
├── phonebook.cpp         # Main source code for the phonebook application
├── phonebook.txt         # Data file that stores names and phone numbers (if created)
└── README.md             # Instructions and documentation for the project
Known Issues
The search function is case-sensitive.
There is no input validation for phone numbers (e.g., it does not check for valid phone number formats).
The MAX_NAMES limit is set to 100, so you can't store more than 100 contacts.
Future Improvements
Implement case-insensitive search.
Add input validation for phone numbers.
Increase the maximum number of contacts or use dynamic memory allocation.
Add a feature to delete contacts.
License
This project is free to use and modify.
