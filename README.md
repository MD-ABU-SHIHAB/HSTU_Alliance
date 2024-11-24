 
HSTU ALLIANCE
LEVEL-3 SEMESTER-I PROJECT REPORT
COURSE CODE: CSE 305 COURSE TITLE: SOFTWARE ENGINEERING

SUBMITTED BY
MD . ABU SHIHAB (ID: 2102051)

SUBMITTED TO
PANKAJ BHOWMIK
LECTURER, DEPARTMENT OF CSE

DEPARTMENT OF COMPUTER SCIENCE AND ENGINEERING
HAJEE MOHAMMAD DANESH SCIENCE AND TECHNOLOGY UNIVERSITY DINAJPUR-5200

                        TABLE OF CONTENTS
Contents                                                                                                                Page    
Chapter-01—Introduction
1.1	Introduction…………………………………………………..   4
1.2	Background of the project……………………………………   5
1.3	Problem statement…………………………………………....   7
1.4	Significance of the project…………………………………...    8
1.5	Scope of the project………………………………………….    8
1.6	Objectives of the project…………………………………….    9
Chapter-02—Methodology
2.1	Development tools and technologies…………..……………  10
2.2	System design..…………………………………….……….    10
2.3	Implementation process………………………………….....    12
Chapter-03—System overview
3.1	Features of the system…………………………..…………..   13
3.2	User interaction…………………………………….……….   13
3.3	Data management…….………………………………….....    17
Chapter-04—Tasks and activities
4.1	Development  activities……………………………………...  18  
4.2	Test activities……...………………………………………..    18
Chapter-05—Results and discussion
5.1	User feedback……………………………………………...     19
5.2	Future enhancement……………………………………….      19

Chapter-06—Conclusion……………………………………………     20
Chapter-07—Appendices
7.1	References……..…………………………………………..     21
7.2	Source code……….………………………………………..    21



                          











                          CHAPTER-01
   
                        INTRODUCTION

1.1 Introduction
The HSTU Alliance project is a student information management system developed to streamline the way students access and manage their university-related details at Hajee Mohammad Danesh Science and Technology University (HSTU). It simplifies the process of organizing and retrieving essential information such as student ID, hall, faculty, and batch. 
In real-life, such a system is crucial for both students and university administrators. For students, it provides a centralized platform to manage their academic and residential information, ensuring easy access to their data whenever needed.This reduces confusion and makes administrative tasks like hall assignments, faculty details, or batch information more efficient. For the university, the system minimizes manual processes, saves time,and prevents data mismanagement by digitizing and automating key operations.
Upon creating an account, students input critical details including their student ID, name, country, and hall. The login page requires the student ID and password for access. Once logged in, students can explore specific categories like their Zone,which displays the student's country and division, the Hall, which shows their floor and room information, and the Faculty, where they can view their department (e.g. CSE, ECE, EEE). 


1.2 Background of the Project
In today’s digital age, educational institutions face increasing demands for efficient and effective management of student information. Traditionally, student data has been maintained through manual processes or cumbersome database systems, leading to inefficiencies, errors, and difficulties in data retrieval. Hajee Mohammad Danesh Science and Technology University (HSTU) is no exception to these challenges, as it seeks to improve how student information is managed and accessed.
The HSTU Alliance project aims to address these challenges by creating a user-friendly platform that allows students to manage their information and access essential details without relying on complex database systems. 
Here we add screenshot: A diagram that illustrates the traditional vs. proposed system.

                    Figure 1.2.1: Traditional vs Proposed system
Traditional system:
•	Manual Record Keeping:
Paper forms, files, or spreadsheets are used to collect and store student information.
Hard copies and manual logs lead to inefficiencies, errors, and slow access.
•	Database-Centric System:
Heavy reliance on databases like MySQL or Oracle.
Students and staff have to go through multiple layers (front-end > middleware > database) to access or update data.
High resource demand (server setup, maintenance, backup systems, etc.).

Proposed System (HSTU Alliance - File-Based System):
•	File-Based Data Management:
The student information is saved in local files (e.g., text, JSON, or XML files).
No need for a complex database system; direct file read/write operations provide simplicity.
Local storage means quicker access, with fewer system resources required.
•	User-Friendly JavaFX Interface:
The GUI provides an intuitive way for users to manage their accounts, log in, and retrieve categorized student data.
No intermediary layers like traditional database systems. The interface directly interacts with local files. 

Diagram structure:
•	Traditional System:
User Interaction → Interface (Web Forms/Manual Input) → Database Layer (SQL Queries, DB) → Student Data



•	Proposed System (HSTU Alliance):
User Interaction → JavaFX Interface (Create Account, Login, Retrieve Data) → Local File Storage (No database) → Student Data in Local Files
•	Visual Elements:
For Traditional System: Use icons to represent the user, database, forms, and manual logs.
For Proposed System: Use icons for the JavaFX interface, local files, and streamlined data access.






1.3 Problem Statement
Managing student information efficiently is critical for educational institutions to provide timely services to students and maintain accurate records. Current methods often involve outdated manual systems or complex database infrastructures that require significant resources to maintain.These methods can lead to delays in data access, errors in record-keeping, and increased workload for administrative staff.
The HSTU Alliance project aims to resolve these issues by providing a straightforward, local file-based system that facilitates easy data management and retrieval for students and administrators alike. This project eliminates the need for complicated databases while still ensuring organized and accessible student information.



1.4 Significance of the Project
The HSTU Alliance project significantly contributes to improving the management of student information at HSTU. Key aspects of its significance include:
•	Enhanced Data Accessibility: Students can easily access their information without waiting for administrative assistance, promoting a more responsive educational environment.
•	Cost-Effectiveness:  By utilizing local file storage, the project reduces the need for expensive database infrastructure, making it a feasible solution for resource-constrained institutions.
•	Improved Administrative Efficiency: Simplifying the management of student records enables staff to focus on other important tasks, thereby improving overall institutional effectiveness.



1.5 Scope of the Project
The scope of the HSTU Alliance project includes the following features:
•	User Account Management: Students can create accounts with personal information for secure access.
•	Data Retrieval: Users can access categorized data such as zone, hall, and faculty information.
•	Local File Storage: Student data is stored in easily manageable local files instead of complex databases.
•	Basic Security Measures: The system includes password protection to ensure data confidentiality.
1.6 Objectives of the Project
	 Primary Objectives
     The primary objectives of the HSTU Alliance project are:
•	To develop a user-friendly system for managing  student  information      without relying on complex database systems.
•	To provide secure access to student data through a simple     login mechanism.


	 Secondary Objectives
     Secondary objectives include:
•	To enhance the accessibility of student information, allowing for      quicker data retrieval.
•	To reduce the administrative burden of managing student records by automating key processes.



                                    




                                     CHAPTER-02

                        METHODOLOGY

2.1 Development Tools and Technologies
The project is developed using the following tools and technologies:
•	Programming Language: Java, due to its robustness and support for GUI development through libraries like JavaFX.
•	File Handling: Java’s built-in file handling capabilities for reading and writing data to local files.
•	Development Environment: An Integrated Development Environment (IDE) such as IntelliJ IDEA for efficient coding and debugging.

2.2 System Design
The system design focuses on creating a user-friendly interface combined with a robust backend for managing student data. The architecture is based on a local file storage model, which allows for efficient data handling without the overhead of a database.
Add Diagram: A flowchart or diagram showing the system architecture, illustrating the interaction between the user interface and backend logic.
 
                           Figure 2.2.1: Flowchart structure

2.3 Implementation Process
The implementation process followed several key steps:
•	Planning: Defined project requirements and designed the system architecture.
•	Development: Created the user interface and backend logic, ensuring smooth integration between components.
•	Testing: Conducted thorough testing to identify and fix bugs, ensuring the system functions as intended.
•	Deployment: Launched the system for use by students and administrative staff.
 
 
                    Figure 2.3.1: HSTU Alliance UML Diagram
                                    CHAPTER-03

                    SYSTEM OVERVIEW

3.1 Features of the System
The HSTU Alliance system includes the following features:
•	User Account Management: Allows students to create and manage their accounts securely.
•	Secure Login System: Requires student ID and password for authentication, ensuring secure access to personal data.
•	Comprehensive Data Retrieval: Users can access categorized information, including zone, hall, and faculty details, with a search functionality for easy navigation.
•	Local File Storage: Data is stored in structured local files, allowing for easy access and management without a database.



3.2 User Interaction
Users interact with the system through an intuitive GUI that simplifies navigation and data retrieval:
•	Account Creation Page: Users can enter their details to create an account.
•	Login Page: Users authenticate themselves before accessing their information.
•	Dashboard: The main interface where users can select the data category they want to view.

 
                                  Figure-3.2.1: Login page 
 
                         Figure-3.2.2: Create an Account Page
 
                                   Figure-3.2.3: Home Page
 
                        Figure-3.2.4: HSTU Alliance Batch Page
 
                  Figure-3.2.5: HSTU Alliance Faculty Page
 
              Figure-3.2.6: HSTU Alliance Hall Page
 
                Figure-3.2.7: HSTU Alliance Zone Page

3.3 Data Management
The system uses local files to store student information in a structured format. Each record is organized for efficient read/write operations, allowing quick access to data when required.
                                     
                                      CHAPTER-04

                  TASK AND ACTIVITIES

4.1 Development Activities
The main activities during the development included:
•	Requirement Gathering: Collaborating with stakeholders to identify their needs.
•	Designing the UI: Creating a user-friendly interface that caters to student needs.
•	Coding: Implementing the functionalities as per the defined requirements.
•	Debugging: Testing the code and resolving any issues identified during testing.



4.2 Testing Activities
Testing involved several methods:
•	Unit Testing: Individual components were tested to ensure they functioned correctly.
•	User Acceptance Testing: Feedback was gathered from users to ensure the system meets their needs and expectations.

                          CHAPTER-05

               RESULTS AND DISCUSSION

5.1 User Feedback
Feedback collected from users highlighted the system's ease of use and the efficiency of data retrieval. Users appreciated the straightforward interface, which significantly improved their ability to access personal information.



5.2 Future Enhancements
Future enhancements could include:
Integration of more advanced features such as notifications for important updates.
Transitioning to a database system as the user base grows and data complexity increases.




                         CHAPTER-06

                           CONCLUSION

The HSTU Alliance project successfully addresses the challenges of student information management at Hajee Mohammad Danesh Science and Technology University. By providing a user-friendly, secure, and efficient system that utilizes local file storage, the project enhances data accessibility for students and reduces administrative workload. This report underscores the project's importance and its potential for future development.












                         CHAPTER-07

                            APPENDICES

7.1 References
•	https://www.javatpoint.com/javafx-tutorial
•	https://www.jetbrains.com/help/idea/javafx.html




