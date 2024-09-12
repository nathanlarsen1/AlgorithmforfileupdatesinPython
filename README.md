<h1>Apply Filters to SQL Queries</h1>


<h2>Project description</h2>
For this project, I acted as a Cybersecurity Analyst on a security team for an organization. My role involved examining logs in a timely manner by using SQL queries to filter log data related to user logins and employee computers.<br/><br/>

<h2>Retrieve After Hours Failed Login Attempts</h2>
I was tasked with investigating a potential security incident that occurred after 18:00, which was outside of normal business hours. The following code demonstrates how I filtered failed logon attempts during this time using a SQL query.</br></br>
                                                
<p align="center">
<img src="https://i.imgur.com/R1OgQmL.png" height="80%" width="80%" alt="Retrieve After Hours Failed Login Attempts"/>
<br />
<br />
</p>

In the screenshot, you will see the SQL query I used and its output. The query begins by selecting all columns from the log_in_attempts table. It then uses a WHERE clause with an AND operator to filter the results, showing all logon attempts that occurred after 18:00 and were unsuccessful.</br></br>
 
<h2>Retrieve Login Attempts on Specific Dates</h2>

A suspicious event occurred on 2022-05-09. To investigate, I reviewed all login attempts from that day and the previous day. I used SQL filters to create a query that identified all login attempts on 2022-05-09 and 2022-05-08.</br></br>

<p align="center">
<img src="https://i.imgur.com/pAPISSU.png" height="80%" width="80%" alt="Retrieve Login Attempts on Specific Dates"/>
<br />
<br />
</p>

In the screenshot, you will see the SQL query I used and its output. The query begins by selecting all columns from the log_in_attempts table. It then uses a WHERE clause with an OR operator to filter the results, displaying all logon attempts that occurred on '2022-05-09' and '2022-05-08'.</br></br>

<h2>Retrieve Login Attempts Outside of Mexico</h2>

There was suspicious activity with login attempts, but the team determined that this activity didn't originate from Mexico. I needed to investigate login attempts that occurred outside of Mexico. I used SQL filters to create a query that identified all login attempts originating from outside of Mexico.</br></br> 

<p align="center">
<img src="https://i.imgur.com/6BhvCIo.png" height="80%" width="80%" alt="Retrieve Login Attempts Outside of Mexico"/>
<br />
<br />
</p>

In the screenshot, you will see the SQL query I used and its output. The query begins by selecting all columns from the log_in_attempts table. It then uses a WHERE clause with a NOT operator to filter the results, displaying all logon attempts that did not occur in Mexico.</br></br>

<h2>Retrieve Employees in Marketing</h2>

My team needed to perform security updates on specific employee machines in the Marketing department. I was responsible for gathering information on these machines, so I queried the employees table. I used SQL filters to create a query that identified all employees in the Marketing department across all offices in the East building.<br/><br/>

<p align="center">
<img src="https://i.imgur.com/12T6bRK.png" height="80%" width="80%" alt="Retrieve Employees in Marketing"/>
<br />
<br />
</p>

In the screenshot, you will see the SQL query I used and the output from that query. The query starts by selecting all columns from the employees table. Then it uses the WHERE clause with an AND operator to filter the results to output all of the employees in the Marketing department that work in offices in the East Building.</br></br>


<h2>Retrieve Employees in Finance or Sales</h2>

My team needed to perform a different security update on machines for employees in the Sales and Finance departments. I used filters in SQL to create a query that identified all employees in the Sales or Finance departments.<br/><br/>

<p align="center">
<img src="https://i.imgur.com/u0ZR5x9.png" height="80%" width="80%" alt="Retrieve Employees in Finance or Sales"/>
<br />
<br />
</p>

In the screenshot, you will see the SQL query I used and the output from that query. The query starts by selecting all columns from the employees table. Then it uses the WHERE clause with an OR operator to filter the results to output all of the employees in the Marketing department and the Finance department.</br></br>

<h2>Retrieve All Employees Not in IT</h2>

My team needed to make one more update to employee machines. The employees who were in the Information Technology department already had this update, but employees in all other departments needed it. I used filters in SQL to create a query which identified all employees not in the IT department.<br/><br/>

<p align="center">
<img src="https://i.imgur.com/9z5H27r.png" height="80%" width="80%" alt="Retrieve All Employees Not in IT"/>
<br />
<br />
</p>

In the screenshot, you will see the SQL query I used and the output from that query. The query starts by selecting all columns from the employees table. Then it uses the WHERE clause with an NOT operator to filter the results to output all of the employees not in the IT department.</br></br>

<h2>Summary</h2>

In this excerise, I demonstrated the use of SQL used by a Cybersecurity Analyst. Several examples displayed how SQL queries can be used to return information for user logins and user computers. Two different tables were used in these examples. One was log_in_attempts and the other was employees. Four different operators were used to filter out the necessary information for each task. These operators were AND, OR, NOT and LIKE. The percent sign wildcard was also utilized to filter data.

