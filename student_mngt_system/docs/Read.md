# Student Management System

## Project Overview
This is a **Student Management System** implemented in C using **linked lists**.  
It allows creating, adding, displaying, inserting, and deleting student records dynamically.  
The system can also calculate grades based on marks in four subjects.

### Key Features
- Dynamically create a list of students
- Add new student records
- Display all student information
- Calculate grades automatically
- Insert students at beginning, end, or a specific position
- Delete students from beginning, end, or a specific position
- Exit program with proper memory cleanup
- Additional features: sorting and searching

---

## Installation / Setup

### Requirements
- GCC Compiler (Linux/Mac) or MinGW (Windows)
- Make (optional, if using Makefile)

### Steps
1. Clone or download the project.
2. Navigate to the project folder:
   ```bash
   cd StudentManagementSystem
````

3. Compile the project:

**Using Makefile:**

```bash
make
```

**Or manually:**

```bash
gcc src/main.c src/functions.c src/insert.c src/delete.c -I include -o sms
```

4. Run the program:

```bash
./sms
```

---

## Usage Guide

When you run the program, the following menu will appear:

```
-------------------------------------
|          ----Menu----             |
|1 | Create students list           |
|2 | Add_student                    |
|3 | Display_students               |
|4 | Calculate grades of students   |
|5 | Insert modes                   |
|6 | Delete modes                   |
|7 | Exit                           |
-------------------------------------
```

**Menu Options:**

1. Create an initial student list
2. Add a single student
3. Display all students
4. Calculate and display grades
5. Insert a student at beginning, end, or specific position
6. Delete a student from beginning, end, or specific position
7. Exit the program

---

## Project Structure (Tree)

```
.
├── docs/
│   └── Read.md
├── include/
│   └── header.h
├── Makefile
└── src/
    ├── main.c
    ├── functions.c
    ├── insert.c
    └── delete.c
```

---

## Data Structure

**`student` struct:**

* `name[20]` : Student name
* `gender[8]` : Gender
* `roll_no` : Roll number
* `s[4]` : Marks of 4 subjects
* `grade` : Calculated grade
* `next` : Pointer to next node (linked list)

---

## Example Run

```
Enter number of students: 2
Enter Name: Alice
Enter Gender: Female
Enter Roll No: 101
Enter Marks (4 subjects): 90 85 95 80

Enter Name: Bob
Enter Gender: Male
Enter Roll No: 102
Enter Marks (4 subjects): 70 75 65 80

Displaying students:
1. Alice, Female, Roll: 101, Marks: 90 85 95 80, Grade: A
2. Bob, Male, Roll: 102, Marks: 70 75 65 80, Grade: B
```

---

## Troubleshooting

* **Invalid input:** Only numeric values for menu options and marks are accepted.
* **Memory issues:** Ensure the program exits properly to free dynamically allocated memory.
* **Compilation errors:** Include all `.c` files and the header path during compilation.

---

## Version History

* **v1.0:** Initial version with create, add, display, and grade calculation
* **v1.1:** Added insert and delete modes
* **v1.2:** Enhanced grade calculation and menu validation

---

## Feature Updates

1. Sorting of student records
2. Searching for a student by name or roll number

```

---

**Enhancements made:**
- Proper Markdown formatting (headings, code blocks, lists)  
- Clean and readable “Usage Guide” and “Tree Structure”  
- Added “Example Run” section  
- Clearly separated “Troubleshooting”, “Version History”, and “Feature Updates”  

---

```

