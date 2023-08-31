# Task-Management-System
Run the following commands to get started:
git clone https://github.com/BhatnagarSomya13/Task-Management-System.git

virtualenv env
Activate the virtual environment
.\env\Scripts\activate

cd TasManagementSystem
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver

**Overview**
This project is a small task management. It was built using Django and DRF and contains the following:
  Allows new accounts registration, login and logout.
  token-based authentication system.
  Each user can create edit delete any of his task.
  Each user can filter through his tasks (eg. Filter to show only uncompleted task).
  Calculate the ratio between complete and incomplete tasks and export it to a file in (CSV, Excel) format.


In order to achieve all of these results, it is necessary to send the Authorization: Token with each link.


**Authentication**
  Signup 127.0.0.1:8000/accounts/register/
  Login 127.0.0.1:8000/accounts/login/

**CRUD Operations**
  All Tasks 127.0.0.1:8000/me/all/
  Create Task 127.0.0.1:8000/tasks/
  Retrieve specific task 127.0.0.1:8000/tasks/id/ Or 127.0.0.1:8000/me/id/
  Update Task 127.0.0.1:8000/tasks/id/
  Delete Task 127.0.0.1:8000/tasks/id/
  
**Filter Tasks**
  All Completed Tasks 127.0.0.1:8000/me/completed/
  All Incompleted Tasks 127.0.0.1:8000/me/incompleted/

**Export Data**
  Export as CSV 127.0.0.1:8000/export/csv/
  Export as XLS 127.0.0.1:8000/export/xls/
