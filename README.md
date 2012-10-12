SDriver
=======

SQL injection attacks involve the construction of application input data that will result in the execution
of malicious SQL statements. Many web applications are prone to SQL injection attacks.
For preventing this kind of attacks we have implemented SDriver. SDriver/SQL is a type 4 JDBC driver
(native-protocol driver) and it must be placed between the application and its underlying database.
To detect an attack, the driver uses stripped-down SQL queries and stack traces to create SQL statement
signatures that are then used to distinguish between injected and legitimate queries. The driver depends
neither on the application nor on the rdbms and can be easily retroﬁtted to any system. For more check the
corresponding publication