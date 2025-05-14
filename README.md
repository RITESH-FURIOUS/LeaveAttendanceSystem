# LeaveAttendanceSystem

Leave Management System
Overview
The Leave Management System is designed to handle the process of managing employee leave requests. It allows administrators to approve or reject leave requests, and employees to submit their leave applications. This system is built in C and uses file handling for storing employee and leave records.

Features
Employee Registration: Allows for the addition of employee details.

Leave Request Submission: Employees can submit their leave requests specifying the leave type and dates.

Leave Approval/Rejection: Admins can approve or reject leave requests.

Leave Balances: Tracks the available leave balance for each employee.

Leave History: Keeps track of the employee's leave history for reference.

File Handling: All employee and leave data is stored in files for persistent storage.

Requirements
C Compiler: The system is written in C and requires a C compiler (e.g., GCC) to compile and run.

Operating System: Should work on Linux/Unix and Windows with minor adjustments for file paths.

System Components
Employee Struct:

Holds employee information like employee ID, name, position, etc.

Leave Request Struct:

Holds information about leave requests, including type of leave, dates, and approval status.

Functions:

addEmployee(): Adds an employee to the system.

submitLeaveRequest(): Allows an employee to submit a leave request.

approveLeaveRequest(): Admin function to approve or reject leave requests.

viewLeaveHistory(): View the leave history for an employee.

viewLeaveBalance(): View an employee's remaining leave balance.

File Handling:

employees.dat: Stores employee records.

leaves.dat: Stores leave requests and statuses.

Setup and Installation
Clone the repository or download the source code files.

Compile the C program:

bash
Copy
Edit
gcc -o leave_system leave_system.c
Run the program:

bash
Copy
Edit
./leave_system
Usage
After running the system, the following options are available in the menu:

Admin Menu
1. Add Employee: Add a new employee record to the system.

2. View Employee Details: View details of a specific employee.

3. Approve Leave Request: Admin can approve or reject employee leave requests.

4. View All Leave Requests: View all leave requests and their statuses.

Employee Menu
1. Submit Leave Request: Employee can submit a leave request specifying leave type and dates.

2. View Leave Balance: View available leave balance.

3. View Leave History: View the employee's leave history.

File Structure
employees.dat - Stores employee data in binary format.

leaves.dat - Stores leave requests data in binary format.

leave_system.c - Main program file with the leave management logic.

README.md - This file for documentation.

Example Data Format
Employee Data (employees.dat):
plaintext
Copy
Edit
EmployeeID, Name, Position, Department, etc.
Leave Request Data (leaves.dat):
plaintext
Copy
Edit
EmployeeID, LeaveType, StartDate, EndDate, Status (Approved/Rejected)
