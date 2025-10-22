## Data Model in Database Management System

- A database model defines the logical design and structure of a database and defines how data will be stored, accessed and updated in a database management system
- Data Model is the modelling of the data description, data semantics, and consistency constraints of the data. 
- It provides the conceptual tools for describing the design of a database at each level of data abstraction.
- Though there are many data models being used nowadays but the relational model is the most widely used model.
- The data model is used to describe the way information is stored and retrieved from a database.
- It also defines the rules by which the database will operate.
- A data model can be defined as an integrated collection of concepts describing and manipulating data, as well as constraints on the data within an organization. A data model is not just a set of tables: it is a conceptual representation of physical data stored in the database.

### Designing a Data Model
- The first step in designing a data model is to define what kind of data you want to store in your database. This usually involves defining the entities involved in your application. An entity is any object tat exists independently of anything else. You might think about an entity as something like a "person" or an "address".
- Once you've identified all the entities, you need to decide how they relate to each other. In most cases, the answer to this question depends on what type of business process you're modelling.
- The next step is to figure out how those entities will interact with each other. In some applications, you may want to create a single table to hold all the data about a particular entity.
- However, you could also use several tables, where each table holds only part of the data about an individual entity. In addition, you should consider whether you'll need to perform queries across more than one tale. If so, you'll probably need to link them together using foreign key columns.

Once you know the basic _==structure==_ of your data model, you can start thinking about how best to organize it into tables. There are two main approaches: relational databases and hierarchical databases:
- **Relational databases** are organized around a set of tables that share common fields.
- **Hierarchical databases** are organized around a tree-like structure called a hierarchy.

Both approaches allow you to build complex structures quickly, but they do so at the cost of flexibility.

### Why use Data Models?
Data models are extremely useful for any organization as they let business users directly define core business rules. As a result, fewer revisions are required during implementation. It also leads to significant reductions in development time allowing businesses to deliver new businesses and projects faster.

Overall, the advantages of using data models: 
   - Helps to cut costs and deliver products faster
   - It improves business processes significantly
   - Reduces complexity and risks in data handling

### Types of Data Model
- Associative Data Model
- Object-Oriented Model
- Entity-Relationship Model
- Semi-structured Model
- Network Model
- Relational Model
- Hierarchical Model
- Object-Relational Model

#### Hierarchical Model
- This database model organizes data into a tree-like-structure, with a single root, to which all the other data is linked. The hierarchy starts from the root data, and expands like a tree, adding child nodes to the parent nodes.
- In this model, a child node will only have a single parent node.
- This model efficiently describes many real-world relationships like index of a book, recipes, etc,
- In hierarchical model, data is organized into tree-like structure with one-to-many relationship between two different types of data, for example, one department can have many courses, many professors and many students.
![[Hierarchical Database Model.canvas|Hierarchical Database Model]]
##### Features of a Hierarchical Model
1. **One-to-many relationship**: The data here is organized in a tree-like structure where the one=to-many relationship is between the data types. Also, there can be only one path from parent to any node.
2. **Parent-child relationship**: Each child node has a parent node but a parent node can have more than one child node. Multiple parents are not allowed.
3. **Deletion problem**: If a parent node is deleted, then the child node is automatically deleted.
4. **Pointers**: Pointers are used to link the parent node with the child node and are used to navigate between the stored data.
##### Advantages of Hierarchical Model
- It is very simple and fast to traverse through a tree-like structure.
- Any change in the parent node is automatically reflected in the child node so, the integrity of data is maintained.
##### Disadvantages of Hierarchical Model
- Complex relationships are not supported.
- As it does not support more than one parent of the child node so if we have some complex relationship where a child node needs to have two parent node then that can't be represented using this model.
- If a parent node is deleted then the child node is automatically deleted.
#### Network Model
- This is an extension of the Hierarchical model. In this model data is organized more like a graph, and are allowed to have more than one parent node.
- This database model was used to map many-to-many data relationships.
- This was the most widely used database model, before Relational Model was introduced.
![[Network Database Model.canvas|Network Database Model]]
##### Advantages
- The data can be accessed faster as compared to the hierarchical model. This is because the data is more related in the network model and there can be more than one path to reach a particular node. so the data can be accessed in many ways.
- As there is a parent-child relationship so data integrity is present. Any change in a parent record is reflected in the child record.
##### Disadvantages
- As more and more relationships need to be handled, the system might get complex. So, a user must be having detailed knowledge of the model to work with the model.
- Any change like update, deletion, insertion is very complex.

#### Relational Data Model
- This type of model designs the data in the form of rows and columns within a table. Tables are also called relations.
- This model was introduced by E.F Codd in 1970, and since then it has been the most widely used database model, in fact, we can say the only database model used around the world.
- The relational data model is the widely used model which is primarily used by commercial data processing applications.

![[Relational Data Model.canvas|Relational Data Model]]
##### Advantages
- **Simple**: This model is simple as compared to the network and hierarchical model.
- **Scalable**: This model can be easily scaled as we can add as many rows and columns as we want.
- **Structural Independence**: We can make changes in database structure without changing the way to access the data. When we can make changes to the database structure without affecting the capability of the DBMS to access te data, we can say that structural independence has been reached.
##### Disadvantages
- **Hardware Overheads**: For hiding the complexities and making things easier for the user, this model requires more powerful computers, hardware and data storage devices.
- **Bad Design**: The relational model is very easy to design and use, so the users don't need to know how the data is stored in order to access it. This ease of design can lead to the development of a poor database which would slow down if the database grows.
> _But all these disadvantages are minor as compared to the advantages of the relational model. These problems can be avoided with proper implementation and organization._

#### Entity-Relationship Data Model
- Entity-Relationship Model or simply ER Model is a high-level data model diagram.
- In this model, we represent the real-world problem in pictorial form to make it easy for the stakeholders to understand.
- It is also very easy for the developers to understand the system by just looking at the ER diagram.
- We use the ER diagram as a visual tool to represent an ER Model.

ER diagrams have the following three components:
1. **Entities**: Entity is a real-world thing. It can be a person, place, or even a concept. Example: Teachers, Students, Course, Building, Department, etc, are some of the entities of a School Management System.
2. **Attributes**: An entity contains real-world properties called attributes. These are the characteristics of that entity. For example, the entity teacher has the properties, teacher id, salary, age, etc.
3. **Relationship**: Relationship tells how two entities are related. For example, a teacher works for a department.
![[Entity-Relationship Data Model.canvas|Entity-Relationship Data Model]]
##### Advantages
- **Simple**: Conceptually ER Model is very easy to build. If we know the relationship between the attributes and the entities we can easily build the ER Diagram for the model.
- **Effective Communication Tool**: This model is used widely by the database designers for communicating their ideas.
- **Easy Conversion to any Model**: This model maps well to the relational model and can be easily converted to relational database by putting the elements in a table. This model can also be converted to any other model like network, hierarchical, etc.
##### Disadvantages
- **No industry standard for notation**: There is no industry standard for developing an ER model. So one developer might use notations which are not understood by other developers.
- **Hidden information**: Some information might be lost or hidden in the ER model. As it is a high-level view so there are chances that some details of information might be hidden.
#### Object-Oriented Model (OODB)
- The real-world problems are more closely represented through the object-oriented data model.
- In this model, both the data and relationship are present in a single structure known as an object.
- We can store audio, video, images, etc. in the database which was not possible in the relational model (although you technically can store audio and video, it is generally advised not to).
- In this model, two or more objects are connected through links. We use this link to relate one object to other objects.
![[Object-Oriented Data Model.canvas|Object-Oriented Data Model]]
> In the example above, we have two objects (Employee and Department). All the data is contained in a single unit (object), including their attributes like name, job title, etc. for employees, and department ID, department name for department. These two objects are linked because of the one common attribute they share-- the Department ID. The communication between the two objects is done through this common identification. This is the representation of the physical model of the Object-oriented data model.
##### Advantages
- **Natural Modeling**: OODBs excel at representing real-world entities and their relationships.
- **Complex Object Handling**: OODBs can handle complex data types beyond the simple scalar values. They can store multimedia content, documents, and other intricate data structures within objects.
##### Disadvantages
- **Limited Adoption**: OODBs haven't achieved the same level of widespread adoption as relational models. This can lead to a smaller pool of developers experienced with OODB management systems and potentially limit the choice of tools and resources available.
#### Object Relational Data Model
- As the name suggests, it is a combination of both the relational model and the object-oriented model.
- This model was built to fill the gap between object-oriented model and the relational model.
- We can have many advanced features like we can make complex data types according to our requirements using the existing data types.
- The problem with this model is that this can get complex and difficult to handle. So, proper understanding of the model is required.
#### Semi-Structured Data Model
A semi-structured model is a modified version of the relational model, allowing for greater flexibility in representing data. It is impossible to distinguish between schema and data in this model because this model is based on the assumption that certain entities might have attributes that are missing. In contrast, other entities may include an additional attribute.

**Example**: An online news website stores information about news articles. The fixed attributes can be in the Authors Table (Article ID, Title, Author ID, Publication Date) and the Articles Tale(Author ID, Name, Bio).

However, the news website might also want to store additional information about each article that doesn't fit neatly into predefined columns. This could include:
- A list of relevant keywords (tags) for better searchability.
- Links to related articles.
- Social media reactions (likes, shares) associated with the article (if applicable).
- Geolocation data if the article is about a specific location.
The additional information can be represented in a semi-structured format.
#### Associative Data Model (ADM)
An associative model is a model with the data divided into two components- entity and association. Everything with an independent existence is termed an _entity_, and the relation between the entities is called a connection or _association_.

The data is further divided into items and links:
- **Items**: An item contains a name and an identifier (specific numerical value).
- **Link**: The link comprises the source, verb, subject, and unique identifier.
**It's a more intuitive way of representing entities with an inherent relationship**. Think of it as a way to model data that captures the "who connects to whom" directly within the entities themselves.
#### Flat Data Model
- A flat data model is a very basic way of storing data in a DBMS. It's like a simple spreadsheet with rows and columns. Imagine a single table with columns representing different data point (e.g., name, age, etc.) and rows representing individual records (e.g., entries for each customer).
- **Think of it as a flat list with no hierarchy or connections between entries**. It's a good starting point for simple data storage, but for anything more complex, relational model (with tables linked through relationships) are more efficient.