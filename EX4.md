# Ex. No: 4 Creating Procedures using PL/SQL

### AIM: To create a procedure using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

### Program:
Create Table :
```sql
 create table employee1(Emp_id NUMBER primary key ,Ename varchar (100) , Dept varchar(20) , Salary NUMBER);
```
Create Procedure :
```sql
1  create or replace procedure insert_emp_data as
2  begin
3  insert into employee1(Emp_id,Ename,Dept,Salary)
4  values(1,'Kothai', 'HR' , 50000);
5  insert into employee1(Emp_id,Ename,Dept,Salary)
6  values (2,'Mithra Mukundaa' , 'IT',50000);
7  insert into employee1(Emp_id,Ename,Dept,Salary)
8  values (3,'Nethraa J' , 'Finance',50000);
9  insert into employee1(Emp_id,Ename,Dept,Salary)
10  values (4,'Lekhashree K' , 'IT',50000);
11  commit;
12  end;
13  /
```
Call Procedure :
```sql
1  begin
2  insert_emp_data;
3  end;
4  /
```
Display Table:
```sql
1  select * from employee1;
```
  
### Output:
![image](https://github.com/KothaiKumar/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/121215739/54f1064d-ad31-41f2-8d27-4a3ba89fcb7c)

![image](https://github.com/KothaiKumar/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/121215739/b353f0bb-91a6-42e0-a9bc-d0a6d8471d41)


### Result:
Thus, a procedure is created using PL/SQL.
