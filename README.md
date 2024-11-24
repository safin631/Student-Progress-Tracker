# **Student Progress Tracker**

## **Introduction**

The *Student Progress Tracker* is a Java-based software system designed to monitor and manage student performance in educational institutions. This system allows teachers, administrators, and students to track grades, attendance, and assignments, and generate progress reports.

By following the Software Development Life Cycle (SDLC), this project ensures a systematic and efficient approach to software development, delivering a high-quality product that meets user requirements.

---

## **Software Development Life Cycle (SDLC)**

The development process for the *Student Progress Tracker* adheres to the following SDLC stages:

### 1. **Planning**
   - **Objective**: Define the project scope, identify stakeholders, and allocate resources.
   - **Activities**:
     - Establish project goals: Enable grade tracking, assignment management, and progress reporting.
     - Identify stakeholders: Teachers, students, administrators.
     - Allocate resources: Developers, testers, tools, and infrastructure.
     - Define project timelines and deliverables.

### 2. **Requirements Analysis**
   - **Objective**: Gather and analyze requirements from stakeholders to define the system's features.
   - **Activities**:
     - Conduct interviews and surveys with teachers and administrators.
     - Define key features:
       - Grade tracking
       - Assignment management
       - Attendance monitoring
       - Progress report generation
     - Specify functional and non-functional requirements.

### 3. **Design**
   - **Objective**: Create the architectural design and system components.
   - **Activities**:
     - Design the system architecture using object-oriented principles.
     - Define database schema:
       - **Students Table**: Stores student details.
       - **Assignments Table**: Tracks assignments and submission status.
       - **Grades Table**: Tracks grades for each student.
     - Design class diagrams for key components:
       - **Student**: Holds student data and grades.
       - **Assignment**: Represents individual assignments and due dates.
       - **Grade**: Links assignments to students and their scores.
     - Create wireframes for user interfaces.

### 4. **Implementation**
   - **Objective**: Develop the system based on the design specifications.
   - **Activities**:
     - Write code for core functionalities in Java.
     - Implement modules for:
       - Adding, editing, and deleting student records.
       - Adding and tracking assignments and grades.
       - Generating and displaying progress reports.
     - Ensure proper integration between the frontend and backend.

   **Example Code Snippet**:
   ```java
   class Student {
       private int studentId;
       private String name;
       private HashMap<String, Integer> grades;

       public Student(int id, String name) {
           this.studentId = id;
           this.name = name;
           grades = new HashMap<>();
       }

       public void addGrade(String assignment, int grade) {
           grades.put(assignment, grade);
       }

       public HashMap<String, Integer> getGrades() {
           return grades;
       }
   }
