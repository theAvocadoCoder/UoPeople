This is a collection of conceptual tools for describing data, data r/ships, data semantics, and consistency constraints. It is the underlying structure of the database.

## Hierarchical Model
- Organizes in a tree structure. Each entity has only one parent but may have several children.
- Ultimate parent is known as the root.
- No sibling relationships.
#### Advantages
- High speed of access to large datasets.
- Data security. (First model to offer this)
- Efficiency.
- Linear type data storage (e.g., tape). Great for one-to-many relationships, e.g., assembly plants and employee organization in corporations.
#### Disadvantages
- Implementation complexity.
- Database management problems.
- Lack of structural independence.
- Slow when searching lower entities. Not ideal for sophisticated r/ships.
- Tape advantage is as obsolete as the linear storage method.
- No support for complex r/ships.

## Network Model
Aka CODASYL Data Model. Based on directed graph theory. Replaces hierarchical tree with graph, allowing for more general connections among the nodes.
#### Advantages
- Conceptual simplicity.
- Capability to handle more relationship types.
- Data independence.
#### Disadvantages
- Detailed structural knowledge is required.
- Lack of structural independence.

## Object-Oriented Model
Obj DBMSs add database functionality to object programming languages, e.g., C++, Java, etc. Extend semantics to provide full DB programming capability while retaining native language compatibility.
#### Advantages
- Apps require less code
- Apps use more natural data model
- Code is easier to maintain
- Higher performance management of objs and complex inter r/ships between objs.
- OO features improve productivity.
- Data access is easy.

## Relational Model
Introduced by E. F. Codd in 1970. Represents data in 2-D  tables.

### Characteristics of Relational Model
- Eliminated parent-child r/ship. Represents data as row/column tables.
- Each table is an independent entity.
- Built in support for query languages, e.g., SQL, ANSI, etc.
- Based on set theory.
- UI is non-procedural. Only what needs to be done is specified.

### E. F. Codd's Laws for a Fully Functional Relational DB
- **Rule 0: Foundation rule**: Must qualify as relational both as a DB and as a MS.
- **Rule 1: The information rule**: All info represented as values in a table.
- **Rule 2: The guaranteed access rule**: All data logically accessible through combo of table name, pry key value and col name.
- **Rule 3: Systematic treatment of null values**
- **Rule 4: Active online catalog based on the relational model**
- **Rule 5: The comprehensive data sub-language rule**
- **Rule 6: The view updating rule**s
- **Rule 7: High-level insert, update and delete**.
- **Rule 8: Physical data independence**
- **Rule 9: Logical data Independence**
- **Rule 10: Integrity independence**: constraints must be defined and separate.
- **Rule 11: Distribution independence**
- **Rule 12: The non subversion rule**

### Principle Components of Relational Model
1. **Data Structure**
2. **Data Integrity**
	- Domain constraints
	- Referential integrity
	- Entity integrity
	- Enterprise constraints.
3. **Data Manipulation**

### Advantages
- Structural independence
- Conceptual simplicity
- Design, implementation, maintenance and usage ease
- Good for adhoc requests
- It is simpler to navigate
- Greater flexibility

### Disadvantages
- Significant hardware and software overheads
- Not as good for transaction process modeling as hierarchical and network models
- May have slower processing than hierarchical and network models