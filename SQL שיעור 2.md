# SQL Lesson 2
#### יצירת database:
```sql
CREATE DATABASE school;
```
#### DB-שימוש ב 
```sql
USE school;
```
#### יצירת טבלה
```sql

USE school;

CREATE TABLE teacher(
	ID INT,
	Name NVARCHAR(20),
	Profession NVARCHAR(20)
)
```
#### אילוצים
###### NOT NULL - אסור שהעמודה תהיה ריקה
```sql
NOT NULL 
```
```sql

USE school;

CREATE TABLE profession(
	ID INT NOT NULL,
	Name NVARCHAR(20) not null,
	LessonsInWeek int
)
```
#### הכנסת מידע לטבלה
insert into - הכנס לטבלה
בתוך סוגריים לאחר שם הטבלה נכתוב את העמודות
values - ערכים
בתוך כל סוגריים נכתוב את השורות. 
```sql

USE school;

INSERT INTO profession(ID,Name,LessonsInWeek)
values(1,'Math',6),
	(2,'Biolgy',2),
	(3,'C',7),
	(4,'Linux',5)
```
#### הצגת הנתונים שבטבלה
###### * = all
```sql
SELECT * FROM profession;
```