# Fall 2024 Principles of Databases — Assignment 4

* **Do not start this project until you’ve read and understood these instructions. If something is not clear, ask.**

---

## ❖ Introduction ❖

For this assignment, you will write responses to nine questions based on different topics from our textbook, *Database Systems — The Complete Book* and to one question based on your notes. Reply to each question in the provided region using Markdown syntax.

---

## ❖ Questions ❖

### 1. [2.4] What is the difference between a Cartesian Product, a Natural Join, and Theta-Joins?

A Cartesian Product takes two sets and combines them by pairing each tuple from one set with the other in every possible combination. 
If the two sets have an attribute in common, the attribute can be disambiguated by using the the names of the sets before the attribute name. 

A Natural Join joins two sets by pairing tuples with one set to the other only if their attributes they have in common have matching values. 
The same tuple from one set can be paired with multiple tuples from the other set. 
Tuples that can't pair with another tuple from the other set are called dangling tuples. 

A Theta-Join is like a fancy version of a Cartesian Product that uses a condition to select certain tuples from the result of a Cartesian
Product to make the combined relation. 

### 2. [2.5] What is a Referential Integrity Constraint?

A Referential Integrity Constraint is a kind of constraint that says one value that exists somewhere must also exist in another, related place.
More specifically, a value that exists in an attribute of a tuple in some relation would also exist in an attribute of a tuple in a different 
relation. 
One or more attributes can be involved when defining a Referential Integrity Constraint. 

###  3. [2.5] What is a Key Constraint?

A key constraint restricts what information in an attribute can match between two tuples. Multiple attributes can be used to define a key constraint. 

### 4. [4.1] What is an Entity/Relationship Model? What purpose does it serve in the process of creating/designing databases?

An Entity/Relationship Model is a visual representation of the structure of a database. Its purpose is to help give a simplified view of the entity sets, attributes, and relationships
that will be implemented in the databse. Other notation is used to show primary keys, weak entity sets and relationships, 1:m/m:n/1:1 relationships, etc.   

### 5. [4.4] What is a Weak Entity Set?

A Weak Entity Set is a kind of entity set whose key is has at least one attribute that comes from another entity set. 

### 6. [5.2.7; 6.3.8] Explain the concepts of Outerjoin, Natural Right Outer Joins, Natural Left Outer Joins, and Full Outer Joins.

Outerjoins avoid dangling tuples who don't have a matching pair by padding the unmatched attribute with a NULL. The Full Outer Join use NULL padding for both relations being joined. The Right 
Outer Join uses NULL padding for the relation on the right side of argument and vice versa for the Left Outer Join.

### 7. [6.6.3] What is the difference between the SQL command `TRANSACTION` and the execution of any statement in SQL?

The command `TRANSACTION` allows the database programmer to group multiple statements together into a single transaction. They can then use either the `COMMIT`
or `ROLLBACK` command to either permenantly apply the changes made to the database by the operations or undo the changes so they don't appear. 
Statements that are executed without this command act as single transactions. 

### 8. [8] What is a Virtual View and what are its advantages?

Replace this content with your answer

### 9. [8.3] What is an *index* and what are its advantages?

Replace this content with your answer

### 10. Explain the concept of an MVC, or model, view, controller, framework for designing full stack applications

Replace this content with your answer

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
