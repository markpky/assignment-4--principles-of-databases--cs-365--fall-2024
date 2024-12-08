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

Replace this content with your answer

###  3. [2.5] What is a Key Constraint?

Replace this content with your answer

### 4. [4.1] What is an Entity/Relationship Model? What purpose does it serve in the process of creating/designing databases?

Replace this content with your answer

### 5. [4.4] What is a Weak Entity Set?

Replace this content with your answer

### 6. [5.2.7; 6.3.8] Explain the concepts of Outerjoin, Natural Right Outer Joins, Natural Left Outer Joins, and Full Outer Joins.

Replace this content with your answer

### 7. [6.6.3] What is the difference between the SQL command `TRANSACTION` and the execution of any statement in SQL?

Replace this content with your answer

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
