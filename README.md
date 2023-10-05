# Ex. No: 4 Creating Procedures using PL/SQL

## AIM:
To create a procedure using PL/SQL.

## Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

## Program:
### Create Table :
create table employeee8(Emp_id NUMBER primary key ,Ename varchar (100) , Dept varchar(20) , Salary NUMBER);
### Create Procedure :
```python
1  create or replace procedure insert_emp_data as
2  begin
3  insert into employeee8(Emp_id,Ename,Dept,Salary)
4  values(1,'Devi', 'HR' , 50000);
5  insert into employeee8(Emp_id,Ename,Dept,Salary)
6  values (2,'Yashwanth' , 'IT',50000);
7  insert into employeee8(Emp_id,Ename,Dept,Salary)
8  values (3,'Priya' , 'Finance',50000);
9  insert into employeee8(Emp_id,Ename,Dept,Salary)
10  values (4,'Thara' , 'IT',50000);
11  commit;
12  end;
13  /
```

### Call Procedure :
```python
1  begin
2  insert_emp_data;
3  end;
4/
```

### Display Table:
1  select * from employeee8;

## Output:
![image](https://github.com/MarellaDharanesh/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/118707669/54c8f390-8553-4780-9e21-a0e4986837f9)

![image](https://github.com/MarellaDharanesh/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/118707669/ea468775-95db-4b97-9e00-614989d495db)


## Result:
Thus, a procedure is created using PL/SQL.
