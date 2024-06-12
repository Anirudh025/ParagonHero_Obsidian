# SQL
![[SQL.excalidraw | 900]]

| DDL | DML |
| ---- | ---- |
| CREATE DATABASE | SELECT FROM |
| CREATE TABLE | WHERE |
| ALTER TABLE | ORDER BY |
| FOREIGN KEY | GROUP BY |
| PRIMARY KEY | INNER JOIN |
|  | SUM, COUNT, AVG |
|  | INSERT, DELETE UPDATE |
## DML
``` SQL
''' USAGE IS SELECT * FROM {TABLENAME}; '''


SELECT * FROM PATIENTS;
''' /\ Selecct all data'''

SELECT Patient_ID, Patient_Name FROM PATIENTS;
''' /\ Selecct certain fields'''

SELECT Patient_ID, Patient_Name FROM PATIENTS WHERE {Criteria};
''' /\ Filter by {Criteria}'''

SELECT * FROM PATIENTS  ORDER BY {Field name} '''(add DESC FOR DESCEDNING)''';
''' /\ Sort'''

SELECT * SUM(Height) FROM PATIENTS;
''' /\ Summation of set field'''

SELECT COUNT(Height) FROM PATIENTS WHERE Height < 30;
''' /\ Counts values with height < 30'''
```
***Use website:*** https://sql-practice.com
	**or you can use**** https://sqlzoo.net
<iframe src="https://sql-practice.com"  height=600 width= 1000></iframe>
<iframe src="https://sqlzoo.net"  height=600 width= 900></iframe>
