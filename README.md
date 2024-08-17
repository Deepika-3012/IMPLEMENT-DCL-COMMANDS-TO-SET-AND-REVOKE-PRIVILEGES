# IMPLEMENT-DCL-COMMANDS-TO-SET-AND-REVOKE-PRIVILEGES

AIM:

To implement DCL Commands to set and revoke privileges.

PROCEDURE:

Data control language (DCL) is used to access the stored data. It is mainly used for revoke and to grant the user the required access to a database. In the database, this language does not have the feature of rollback. It is a part of the structured query language (SQL). It helps in controlling access to information stored in a database. It complements the data manipulation language (DML) and the data definition language (DDL).It is the simplest among three commands. It provides the administrators, to remove and set database permissions to desired users as needed. These commands are employed to grant, remove and denypermissions to users for retrieving and manipulating a database.

GRANT Command

It is employed to grant a privilege to a user. GRANT command allows specified users to perform specified tasks

Syntax

GRANT privilege_name on objectname to user;

Here,

privilege names are SELECT,UPDATE,DELETE,INSERT,ALTER,ALL objectname is table name user is the name of the user to whom we grant privileges

REVOKE Command

It is employed to remove a privilege from a user. REVOKE helps the owner to cancel previously granted permissions.

Syntax

REVOKE privilege_name on objectname from user;

Here,

privilege names are SELECT,UPDATE,DELETE,INSERT,ALTER,ALL object name is table name user is the name of the user whose privileges are removing

COMMANDS:

SQL> Grant Create session to student;

SQL> Grant create table to student;

SQL> Connect student/young;

SQL> Connect system/managers;

SQL> Create user staff identified by guru;

SQL> Grant resource to staff;

SQL> Connect staff/guru;

SQL> Select * from staff;

Staff master in a table in the user staff we first log on the staff [SQL> Connectstaff/guru;]

SQL> Grant select insert on staff master to student;

Now log on to student and try the select command

SQL> Connect student/young;

SQL> Select * from staff;

SQL> Grant select, update, delete on student-master to staff;.

SQL> REVOKE SELECT, INSERT ON STUDENT_MASTER from staff;

SQL> REVOKE SELECT ON STUDENT_MASTER from rajan;

RESULT:

Thus the DCL Commands to set and revoke privileges has been executed successfully.
