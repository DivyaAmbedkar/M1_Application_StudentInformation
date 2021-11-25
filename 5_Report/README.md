# REPORT
# Student information System

![StudentInformation](https://user-images.githubusercontent.com/94296796/143388488-ad54912f-6384-496c-ab16-3fd554fe2e53.jpg)

A Simple Software for Student information System that can perform the following operations:
1. Add/Delete the Details of the Students
2. Attendance Monitoring of the students
3. Set/Edit Eligibility criteria for exams
4. Check Eligible Students for Exams
5. Print all the records of the students


## Folder Structure
|Folder|Description|
|:-----|:----------|
|1_Requirement|Documents detailing and research|
|2_Design|Documents regarding design details|
|3_Implementation|All code and documentation|
|4_TestPlanAndOutput|Documents with test plan and procedure|
|5_Report|Project Report|
|6_imagesAndVideos|Project output and videos|


# Requirements 
 ## Introduction
 The primary purpose of school information system Software is to simplify teachers and staff work, by automating all school exam related operations and streamlining their routine tasks.

## Key Features
1. Add/Delete the Details of the Students
2. Attendance Monitoring of the students
3. Set/Edit Eligibility criteria for exams
4. Check Eligible Students for Exams
5. Print all the records of the students

## Approach 
The idea is to form an individual function for each operation. All the functions are unified together with switch cases to form software. Below is the illustration of the functions:
1. execute(): This function will shows the available choices for the software and will perform the following functionality using Switch Statements.
They are add Student Details, Show Eligible Students, delete Student Record, Update Eligibility Criteria, Print Details of Students.

2. add(): This function that get the data from the user and update the list of the students. While adding the student into the list, check for the uniqueness of the Roll Number of the student. Details of the students to be added are: Name of Student, Roll Number, Fees Status, Attendance Record of student.

3. eligibleStudents(): This function shows the previous attendance percentage required for exams and get the data from the user and update the eligibility for the exams. It also updates the fee status required for the eligibility of exams by iterating over the List of the student records and for every student check the attendance percentage is above the percentage required and fee status of the student.

4. print_student(): This function iterate over the list of students and print the details of the student.

5. delete(): This function get the student roll number to delete the student record and update the student’s list.

## SWOT ANALYSIS



## 4W's and 1'H

## Who: 
This software can be used in all schools, colleges and universities.
## What:
The system ensures overall student development, along with eliminating the tedious admin tasks. It is easy to maintain and manage an ERP system than a hand written file.
## Where:
This software can be used all across the globe.
## How:
Enhance the efficiency of schools in meeting their requirements and capabilities. Communicate the key information and advice for good ecosystem.

# Detail Requirements
## High level requirements

|ID	  |Description 	                                  |Category  |Status    |
|:----|:----------------------------------------------|:---------|:----------|
|HR01	|User should be able to add a new student record| Technical|Implemented|
|HR02	|User should be able to update a student record	| Technical|Implemented|
|HR03	|User should be able to delete a patient record	| Technical|Implemented|
|HR04	|User should be able to read data from a file	  |Technical|Implemented|

## Low level requirements
|ID   |Description                                                                                            |HLR ID    |Status      |
|:----|:------------------------------------------------------------------------------------------------------|:---------|:-----------|
|LR01 |While adding the student into the list, check for the uniqueness of the Roll Number of the student.    |HR01      |Implemented|
|LR02 |User should get the data from the students and update the eligibility for the exams. User should  updates the fee status required for the eligibility of exams.       |HR02      |Implemented|                                        
|LR03 |User should get the student roll number to delete the student record and update the student’s list.    |HR03      |Implemented|
|LR04 |User should be able to read the read the data by searching student's roll number or by printing all the available records.|HR04  |Implemented|

# Design 
## High level design
### Architecture Design

![image1](https://user-images.githubusercontent.com/94296796/143389049-29aec099-d0d4-4a25-8f33-9c6c92fa7595.jpg)

## Use case diagram
![image 2](https://user-images.githubusercontent.com/94296796/143389205-57b1d1b9-3de3-4c0e-ab0a-89f6613e110c.jpg)

## Low level design 

### State diagram 

![image4](https://user-images.githubusercontent.com/94296796/143389246-867d1a99-b641-4e74-a277-e34b53828ad4.jpg)

![image3](https://user-images.githubusercontent.com/94296796/143389294-ea56de21-c7bf-435d-9d49-48322ab47255.jpg)

## TEST PLAN

|Test ID|Description|Expected I/P|Expected O/P|Actual O/P|Type of Test|
|:------|:----------------------------------|:-------|:-------|:--------|:------|
|T_01   |Checking add_student_record function to determine whether the function is accepting student information or not| Student details|Accept the details|Accept the detials|Requirement based|
|T_02   |Checking check_eligibility function to determine whether the function is providing eligible student list or not|Student details|Eligible students|Eligible students|Scenario based|
|T_03   |Checking change_eligibility function to determine whether the funcion is able to change the required eligibility criteria or not|New eligiblity criteria|Updated eligiblity criteria|Updated eligibility criteria|Scenario based|
|T_04|Checking reject_eligibility function to determine whether the function is able delete uneligible students or not|Student details|Eligible criteria|Elegible Criteria|Requirement based|
|T_05|Checking delete_student_record function to determine whether the function is able to delete required students or not|Student details|Deleted information|Deleted information|Requirement based|



