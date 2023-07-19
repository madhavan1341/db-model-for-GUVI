# db-model-for-GUVI

Guvi Zen Class Database Model:

Students:

StudentID  (Primary Key)
Name (VARCHAR)
Email (VARCHAR)
Phone Number (VARCHAR)
Date of Birth (VARCHAR)
Address (VARCHAR)
Any other relevant student details
Instructors:

InstructorID (Primary Key)
Name (VARCHAR)
Email (VARCHAR)
Phone Number (VARCHAR)
Specialization/Area of expertise (VARCHAR)
Any other relevant instructor details
Classes:

ClassID (Primary Key)
Class Name (VARCHAR)
Class Description (VARCHAR)
Start Date (VARCHAR)
End Date (VARCHAR)
InstructorID (VARCHAR) (Foreign Key referencing the Instructors table)
Any other relevant class details
Enrollments:

EnrollmentID  (Primary Key)
StudentID (VARCHAR) (Foreign Key referencing the Students table)
ClassID (VARCHAR) (Foreign Key referencing the Classes table)
Enrollment Date (VARCHAR)
Assignments:

AssignmentID  (Primary Key)
ClassID (VARCHAR) (Foreign Key referencing the Classes table)
Assignment Name (VARCHAR)
Description (VARCHAR)
Due Date (VARCHAR)
Maximum Score (VARCHAR)
Submissions:

SubmissionID (Primary Key)
AssignmentID (VARCHAR) (Foreign Key referencing the Assignments table)
StudentID (VARCHAR) (Foreign Key referencing the Students table)
Submission Date (VARCHAR)
Submission Text/Link (VARCHAR)
Score (VARCHAR)
