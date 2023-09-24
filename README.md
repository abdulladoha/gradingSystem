# gradingSystem
A C# console application that calculates and displays the average grade for a group of students based on their exam scores. Here's a step-by-step explanation of what the code does:

Variable Initialization:

Several variables are initialized at the beginning of the program:
currentAssignments: The total number of graded assignments (set to 5).
Arrays of exam scores for four students: sofiaScores, andyScores, emmaScores, and loganScores.
An array of student names: studentNames.
An array to store student scores: studentScores (initially empty).
Report Header:

The program writes a report header to the console with the text "Student" and "Grade" separated by a tab character.
Loop Through Student Names:

The code enters a foreach loop that iterates through the studentNames array, which contains the names of the four students.
Processing Each Student:

Inside the loop, the code processes each student one by one.
It assigns the current student's name to the currentStudent variable.
It selects the appropriate array of exam scores for the current student based on their name using a series of if-else statements.
Calculating Student Grade:

The code initializes sumAssignmentScores to zero to keep track of the sum of exam scores for the current student.
It also initializes currentStudentGrade to zero, which will store the calculated average grade for the student.
It then enters a nested foreach loop to iterate through the exam scores for the current student.
Inside the inner loop, it adds each exam score to sumAssignmentScores to calculate the total score.
Average Grade Calculation:

After summing up all the exam scores, it calculates the average grade for the current student by dividing sumAssignmentScores by currentAssignments. The result is stored in the currentStudentGrade variable.
Displaying Student Information:

The program uses Console.WriteLine to display the current student's name (currentStudent) and their calculated grade (currentStudentGrade) in a tabular format.
The "\t\t" sequences are used to align the text in columns.
Repeat for Next Student:

The foreach loop continues to the next student in the studentNames array, and the process is repeated for each student.
