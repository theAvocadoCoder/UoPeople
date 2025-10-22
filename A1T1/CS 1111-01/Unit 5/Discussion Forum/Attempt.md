Part 1

In some way, all aspects of our lives, personal and professional, are touched by databases (Vidhya et al., 2016). Today, a database-driven approach to data management is not just something that gives a business an edge. It is more of a necessity.

Traditional file systems favored multiple data files, such as comma separated values (CSV), each recorded and managed by its own application program (Vidhya et al., 2016).

A database comprises of:
-  an entity or a relation, which maps to a real-world concept; 
- its attributes or properties; 
- the tuples or records which are instances of this entity; and 
- its relationship to other entities (The Knowledge Adda, 2025; NS lectures, 2023).

This unified approach to data storage avoids data redundancy, data isolation, and data integrity issues, making data storage and retrieval convenient and efficient (Vidhya et al., 2016).

This is especially useful for a business when keeping track of customer information. A DBMS will allow information like customer orders and addresses to be stored as different entities in the same location. Retrieving addresses when making deliveries would take a single query, rather than having to manually search or create a special program for that purpose.

Part 2

Over the years, models for multiple DBMSs have been proposed and explored. Some, like the hierarchical DBMS have phased out of relevance, however, they all have their contextual uses.

The hierarchical DBMS model employs a tree like structure for representing data (Vidhya et al., 2016). In this model, there can be only parent-child relationships with each child having only one parent. This model was the first to offer data security, and is fast and efficient.

Unfortunately, it is not suited for sophisticated or complex relationships due to its strict hierarchical structure. It is not ideal for most businesses today.

Network DBMS extended this model to support sibling relationships (The Knowledge Adda, 2025), moving from a tree structure to a graph. It introduced many-to-many relationships, allowing for faster access, while keeping data integrity.

The system has complex operations and gets more complex the larger the database grows. It is great for processing transactions, but might not be worth it for more mundane use.

Relational DBMS is the most widely-adopted model. It represents data in two-dimensional (rows and columns) tables. It is based on set theory and has built-in support for query languages (Vidhya et al., 2016). This model is simple, flexible, and has structural independence.

The drawback of this model is that it is costly in terms of hardware and also software. For most small businesses, however, it is a worthwhile investment. It is well-suited for the data needs of a business today.

Part 3

Data Abstraction refers to how complex details of the workings of the database are hidden away from the user. This facilitates focusing on business logic.

Data abstraction happens in three levels (Vidhya et al., 2016). The lowest level, the physical level, describes how data is stored. The next level is the logical level, describing what data is stored, and the existing relationships among the data. The highest level, the view level, describes only part of the entire database.

This abstraction makes it easier for the end user, who interacts with the view level, to navigate the DBMS. An example of this user might be the customer who interacts with their profile settings and edits their data. On the logical level, you have the programmer or the database administrator as users. 

Data independence (DI) is the ability to modify schema definition in one level without affecting next higher level (Vidhya et al., 2016). This happens in two levels; physical and logical. The former is occasionally for performance improvements and involves modifying the physical schema without the application programs getting rewritten.

Logical DI is much harder to achieve. It is the modification of the conceptual schema and is necessary whenever the logical structure of the database is altered. Application programs are dependent on this and will often have to be rewritten.

During database migrations, data independence will ensure that applications stay functional. Otherwise, the business may lose money.



References
1. Vidhya, V., Jeyaram, G., & Ishwarya, K. (2016). _Database management systems_. Alpha Science International.
2. NS lectures. (2023, July 1). _what is database, dbms, advantages, disadvantages , characteristics, features database tasks in dbms_ [Video]. YouTube. https://youtu.be/T5HHW72iZpM/
3. The Knowledge Adda. (2025, January 30). _RDBMS - L5 : Data models | Data Abstraction | Data Independence | Logical vs Physical Independence_ [Video]. YouTube. https://youtu.be/nUv1HnONw6Y/

Question
NoSQL is a flexible alternative to SQL, but not a replacement. Could this be because NoSQL is unable to truly replace SQL, or is it a case of slow adoption?