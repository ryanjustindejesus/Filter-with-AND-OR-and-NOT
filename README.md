<h1>Filtering with AND, OR, and NOT </h1>



<h2>Description</h2>
In this lab, I used the AND, OR, and NOT operators in SQL to filter for information. I used SQL to get specific information about employees, their machines, and the departments they’re in. I will be using the MariaDB shell to run SQL queries.
<br />


<h2>Practical experience gained in this Lab</h2>

- <b>Running SQL queries to retrieve information from a database</b> 
- <b>Applying AND, OR, and NOT operators to filter SQL querires</b>

<h2>Environments Used </h2>

- <b>Qwiklabs</b> 

<h2>Lab walk-through:</h2>

<h2>Task 1: Retrieve after hours failed login attempts </h2>
In this task, my team is investigating failed login attempts that were made after business hours. I want to retrieve this information from the login activity. I will be identifying all unsuccessful attempts after 18:00.
<br/> <br />
(1) I used the command "SELECT * FROM log_in_attempts WHERE login_time > '18:00' AND success = FALSE;" to retrieve the failed login attempts that occured after business hours.
<br/> <br/> <p align="center">
<img src="https://imgur.com/pgSosJ3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 2: Retrieve login attempts on specific dates </h2>
In this task, my team is investigating a suspicious event that occurred on '2022-05-09'. I want to retrieve all login attempts that occurred on this day and the day before ('2022-05-08').
<br/> <br />
(2) I used the command "SELECT * FROM log_in_attempts WHERE login_date = '2022-05-09' OR login_date = '2022-05-08';" to retrieve the failed login attempts on the specified days.
<br /> <br /> <p align="center">
<img src="https://imgur.com/pJD3z2v.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 3: Retrieve login attempts outside of Mexico </h2>
In this task, my team is investigating logins that did not originate in Mexico, and I need to find this information.
 <br/> <br/>
(3) I used the command "SELECT * FROM log_in_attempts WHERE NOT country LIKE 'MEX%';" to retrieve login attempts that did not originate in Mexico.
<br/> <br/> <p align="center">
<img src="https://imgur.com/Br3vc1M.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 4: Retrieve employees in Marketing </h2>
In this task, my team is updating employee machines.
 <br/> <br/> 
(4) I used the command "SELECT * FROM employees WHERE department = 'Marketing' AND office LIKE 'East%';" to retrieve information about employees in the 'Marketing' department who are located in all offices in the East building (such as 'East-170' or 'East-320').
<br/> <br/>  <p align="center">
<img src="https://imgur.com/V6j2JpV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 5: Description </h2>
In this task, my team needs to perform a different update to the computers of all employees in the Finance or the Sales department, and I need to locate information on these employees.
 <br/> <br/> 
(5) I used the command "SELECT * FROM employees WHERE department = 'Finance' OR department = 'Sales';" to retrieve records for employees in the 'Finance' or the 'Sales' department.
<br/> <br/>  <p align="center">
<img src="https://imgur.com/daylUj4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 6: Retrieve all employees not in IT </h2>
In this task, my team needs to make one more update. This update was already made to employee computers in the Information Technology department. The team needs information about employees who are not in that department. 
 <br/> <br/> 
(6) I used the command "SELECT *FROM employees WHERE NOT department = 'Information Technology';" to retrieve records for employees who are not in the 'Information Technology' department.
<br/> <br/>  <p align="center">
<img src="https://imgur.com/fftB1wu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />
