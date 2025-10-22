- Data refers to known facts that can be recorded that have implicit meaning.
- When data is processed, organized, structured or presented in a given context, it becomes information.
- A database is a collection of data.
- Database Management System refers to a collection of interrelated data and a set of programs whose primary goal is to provide a way to store and retrieve database information that is both _convenient_ and _efficient_.
- Database System refers to the database and DBMS collectively. It allows users to perform CRUD operations on the computerized data files it keeps record of.

### Structure of DBMS
- The translation from the conceptual schema to the database description is performed using a Data Definition Language (DDL) or a graphical or textual design interface.
- The database description is then used to translate data from its logical representation to its physical representation and vice versa.

### Applications of Database
- Databases touch all aspects of our lives. Examples are banking, airlines, universities, sales, online retailers, manufacturing, human resources.

### Classification of Database Management System
1. **Passive Database Management System**: Users query the current state of the DB and retrieve the information currently available in the DB. Program-driven, e.g., traditional DBMS.
2. **Active Database Management System**: Users specify to the DBMS what info they need. If info is available, DBMS actively monitors the arrival of the desired information. Scope goes beyond past and present to include future data. It is data- and event-driven.

## File Processing System
- FPS is a collection of files and programs that access or modify electronic files. it is supported by a conventional operating system. System needs different apps to extract and add records to files. Each program manages and defines its own data.
### Drawbacks of Conventional FPS
- Data Redundancy and Inconsistency
- Difficulty in Accessing Data
- Data Isolation
- Concurrent Access Anomalies
- Security Problems
- Integrity Problems
- Atomicity Problems

## Advantages of DB
- Controlling Data Redundancy
	- Data is recorded at only one place and is not duplicated.
- Data Consistency
- Data Sharing
- Data Integration
- Integrity Constraints
	- AKA consistency rules. Applied to DB to ensure correct data entry.
	- May be applied to data item within single record or r/ship btwn records.
- Data Security
- Data Atomicity
	- This ensures that tasks that involve multiple steps are completed entirely, or not at all. Failure to complete is handled with a rollback.
- Development of Application
- Creating Forms
- Report Writers
- Control over Concurrency
- Backup and Recovery Procedures
- Data Independence
- Advanced Capabilities

## Disadvantages of DB
- Cost of Hardware and Software
- Cost of Data Conversion
- Cost of Staff Training
- Appointing Technical Staff
- Database Failures

## Views of Data
Major purpose of database system is to hide details of data storage and maintenance, providing users with an abstract view of the data.

### Data Abstraction
Three layers of data abstraction:
- **Physical**. Lowest. Describes complex low-level data structures in details. The "how".
- **Logical**. Middle. Describes stored data and existing relationships. The "what".
- **View**. Highest. Describes only part of entire DB.

### Data Independence
Ability to modify schema definition in one level without affecting next higher level. Two levels:
- **Physical**. Modify physical without apps being rewritten. Occasionally necessary for performance improvements.
- **Logical**. Modify conceptual without apps being rewritten. Necessary whenever logic structure of DB is altered. Much harder to achieve than physical.

### Instances and Schemas
Instance is the snapshot of the DB at a given point in time. Schema is the overall design of the DB. 3 types:
- Physical
- Logical
- Sub-schema (View level)