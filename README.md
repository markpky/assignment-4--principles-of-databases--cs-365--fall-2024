# Fall 2024 Principles of Databases — Assignment 4

* **Do not start this project until you’ve read and understood these instructions. If something is not clear, ask.**

---

## ❖ Introduction ❖

For this assignment, you will write responses to nine questions based on different topics from our textbook, *Database Systems — The Complete Book* and to one question based on your notes. Reply to each question in the provided region using Markdown syntax.

---

## ❖ Questions ❖

### 1. [2.4] What is the difference between a Cartesian Product, a Natural Join, and Theta-Joins?

A Cartesian Product takes two sets and combines them by pairing each tuple from one set with the other in every possible combination. 
If the two sets have an attribute name in common, the attribute can be disambiguated by using the the names of the sets before the attribute name. 

A Natural Join joins two sets by pairing tuples from one set to the other only if their attributes they have in common have matching values. 
The same tuple from one set can be paired with multiple tuples from the other set. 
Tuples that can't pair with another tuple from the other set are called dangling tuples. 

A Theta-Join is like a fancy version of a Cartesian Product that uses a condition to select certain tuples from the result of a Cartesian
Product to make the combined relation. 

### 2. [2.5] What is a Referential Integrity Constraint?

A Referential Integrity Constraint is a kind of constraint that says one value that exists somewhere must also exist in another related place.
More specifically, a value that exists in an attribute of a tuple in some relation must also exist in an attribute of a tuple in a different 
relation. 
One or more attributes can be involved when defining a Referential Integrity Constraint. 

###  3. [2.5] What is a Key Constraint?

A key constraint restricts what information in an attribute can match between two tuples. Multiple attributes can be used to define a key constraint. 

### 4. [4.1] What is an Entity/Relationship Model? What purpose does it serve in the process of creating/designing databases?

An Entity/Relationship Model is a visual representation of the structure of a database. Its purpose is to help give a simplified view of the entity sets, attributes, and relationships
that will be implemented in the databse. Other notation is used to show primary keys, weak entity sets and relationships, 1:m/m:n/1:1 relationships, etc.   

### 5. [4.4] What is a Weak Entity Set?

A Weak Entity Set is a kind of entity set whose key has at least one attribute that comes from another entity set. This kind of reliance means that for a tuple to be unique from the rest, 
there has to be a reference to another entity set.  

### 6. [5.2.7; 6.3.8] Explain the concepts of Outerjoin, Natural Right Outer Joins, Natural Left Outer Joins, and Full Outer Joins.

Outerjoins avoid dangling tuples who don't have a matching pair by padding the unmatched attribute with a NULL. The Full Outer Join use NULL padding for both relations being joined. The Right 
Outer Join uses NULL padding for the relation on the right side of the argument and vice versa for the Left Outer Join.

### 7. [6.6.3] What is the difference between the SQL command `TRANSACTION` and the execution of any statement in SQL?

The command `TRANSACTION` allows the database programmer to group multiple statements together into a single transaction. They can then use either the `COMMIT`
or `ROLLBACK` command to either permenantly apply the changes made to the database by the operations or undo the changes so they don't appear. 
Statements that are executed without this command act as single transactions. 

### 8. [8] What is a Virtual View and what are its advantages?

Virtual Views are expressions disguised as relations. Virtual Views are created with a name and a definition, which is an SQL query. Virtual Views can help make work on a relation easier and 
quicker to write by wrapping part of what would be a long query into the definition of the Virtual View. Operations done through a Virtual View can be rewritten without it, but are sometimes 
longer and more complicated. 

### 9. [8.3] What is an *index* and what are its advantages?

An index is a kind of data structure that can make searches within a relation faster. It uses a certain kind of binary search tree and is defined by one or more attributes in a 
relation. Queries where we select tuples from a relation based on the attribute that's used to define the index will generate results faster than those without an index. Speed is important 
if there are lots of entries to search through and make comparisons on.  

### 10. Explain the concept of an MVC, or model, view, controller, framework for designing full stack applications

Full stack applications use a combination of technologies to allow a user to view and interact with a database through the web. The model is the database where information is stored. The 
view is what the user sees and can interact with. The controller acts as a mediary between the view and controller by doing things like retrieving information from the model to display in 
the view and taking user input and then turning them into commands to affect the model. 

---

## ❖ Due ❖

Sunday, 15 December 2024, at 10:00 AM.

---

## ❖ Grading ❖

| Item        | Points |
|-------------|:------:|
| Question 1  | `10`   |
| Question 2  | `10`   |
| Question 3  | `10`   |
| Question 4  | `10`   |
| Question 5  | `10`   |
| Question 6  | `10`   |
| Question 7  | `10`   |
| Question 8  | `10`   |
| Question 9  | `10`   |
| Question 10 | `10`   |

---

## ❖ Submission ❖

**NO late submissions will be accepted.**

You will need to issue a pull request back into the original repo, the one from which your fork was created for this project. See the **Issuing Pull Requests** section of [this site](http://code-warrior.github.io/tutorials/git/github/index.html) for help on how to submit your assignment.

**Note**: This assignment may **only** be submitted via GitHub. **No other form of submission will be accepted**.
