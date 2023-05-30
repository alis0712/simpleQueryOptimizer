# Simple Query Optimizer
Query Optimizer

### The goal of this project was to implement a simple query optimization module with graphic user interface. We were allowed to give a limit of 5 tables and simulate a query processing system. For example, one can follow the user interface of https://sqlzoo.net/wiki/SQL_Tutorial, and to develop a similar system. The user may type in a query as in textbox, and may not be in the optimal format. And our system was supposed to do the following:
 
### Rewrite the query into an optimal format.
### Give the query tree in graphic form.
 
For example, the user may give a query as
SELECT EMPLOYEE.EMPNO, POSITION
FROM EMPLOYEE  E,  JOBHISTORY  J
WHERE E. EMPNO = J. EMPNO
AND STARTDATE <= ENDDATE
AND SALARY <= 3000;
 
Here, the unlined part is unnecessary and can be optimized. Therefore, your system should automatically rewrite the query into
SELECT EMPLOYEE.EMPNO, POSITION
FROM EMPLOYEE  E,  JOBHISTORY  J
WHERE E. EMPNO = J. EMPNO
AND SALARY <= 3000;
 
And give the optimal query tree of this query using the knowledge learned from class.
