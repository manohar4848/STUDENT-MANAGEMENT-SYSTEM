Code Explanation:
Structure Definition (struct Student):

Represents a student with fields for id, name, grades (for 5 subjects), and average_grade.
Main Function (main()):

Initializes an array students of struct Student to store up to 50 students.
numStudents keeps track of the current number of students in the array.
It presents a menu-driven interface to:
Register a new student (registerStudent() function).
Edit student information (editStudent() function).
Delete a student (deleteStudent() function).
Exit the program.
Functions:

registerStudent(): Prompts the user to input student details and calculates the average grade before adding the student to the array.
editStudent(): Allows editing of student information based on the provided student ID.
deleteStudent(): Deletes a student based on the provided student ID by shifting subsequent students in the array.
calculateGrades(): Computes the average grade for a student based on their grades in 5 subjects.
Expected Output:
Upon running the program (./a.out assuming compilation), it will display a menu:
markdown
Copy code
Student Management System
1. Register a new student
2. Edit student information
3. Delete a student
4. Exit
Enter your choice:
Registration (1):

Prompts for ID, name, and grades of the new student.
After successful registration, it confirms: "Student registered successfully."
Edit Student Information (2):

Prompts for the student ID to be edited.
If found, allows editing of the student's name and grades.
Confirms: "Student information updated successfully."
If student ID is not found, it prints: "Student not found with ID <id>."
Delete Student (3):

Prompts for the student ID to be deleted.
If found, deletes the student and shifts the array.
Confirms: "Student deleted successfully."
If student ID is not found, it prints: "Student not found with ID <id>."
Exit (4):

Displays: "Exiting program." and terminates the program.
Example Interaction:
Assume the following interaction:

Register a student with ID 1, name "John Doe", and grades 90, 85, 80, 95, 88.
Edit student 1 to change name to "John Smith" and grades to 85, 80, 75, 90, 82.
Delete student 1.
Output might look like this:

yaml
Copy code
Student Management System
1. Register a new student
2. Edit student information
3. Delete a student
4. Exit
Enter your choice: 1

Enter student ID: 1
Enter student name: John Doe
Enter grades for 5 subjects:
Subject 1: 90
Subject 2: 85
Subject 3: 80
Subject 4: 95
Subject 5: 88
Student registered successfully.

Student Management System
1. Register a new student
2. Edit student information
3. Delete a student
4. Exit
Enter your choice: 2

Enter student ID to edit: 1
Enter new name for student: John Smith
Enter new grades for 5 subjects:
Subject 1: 85
Subject 2: 80
Subject 3: 75
Subject 4: 90
Subject 5: 82
Student information updated successfully.

Student Management System
1. Register a new student
2. Edit student information
3. Delete a student
4. Exit
Enter your choice: 3

Enter student ID to delete: 1
Student deleted successfully.

Student Management System
1. Register a new student
2. Edit student information
3. Delete a student
4. Exit
Enter your choice: 4

Exiting program.
