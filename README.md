# Fall 2024 Principles of Databases — Assignment 4

* **Do not start this project until you’ve read and understood these instructions. If something is not clear, ask.**

---

## ❖ Introduction ❖

For this assignment, you will write responses to nine questions based on different topics from our textbook, *Database Systems — The Complete Book* and to one question based on your notes. Reply to each question in the provided region using Markdown syntax.

---

## ❖ Questions ❖

### 1. [2.4] What is the difference between a Cartesian Product, a Natural Join, and Theta-Joins?

The cartesian product of two tables produces a table containing every row of each table, a d is the basic combination of both tables. A natural join combines only tuples from each table that have the same values in common columns (or attributes). Natural Joins exclude repeat tuples. Theta Join combines two tables based on a condition using the comparison oprerators to specify columns.

### 2. [2.5] What is a Referential Integrity Constraint?

Referential Integrity is the concept that in a mutli-way relationship, and arrow from entity set E to entity set F asserts that for any set in F, a related entity set is required to exist in E. Foriegn-Key constraints uphold this concept by asserting that a value apperearing in one relation must also appear in the primary key components of another relation. NOT NULL and CHECK contraints are also used to put restrictions on the values of certain attributes.

###  3. [2.5] What is a Key Constraint?

A Key constraint is a an attribute or set of attributes which does not allow another identical instance of itself. In other words, the key asserts that each tuple must have a unique value for at least one of the attributes in the key.

### 4. [4.1] What is an Entity/Relationship Model? What purpose does it serve in the process of creating/designing databases?

An E/R Model is notation used to descride the schemas of a database. It serves as the basic diagram to determine design aspects like constraints, relationship types (many-to-one, many-to-many, one-to-one), and whether an entity set is weak or strong. For the cretion of schema, the E/R model has a process for the conversion of the model's entity's and relationships into relations. This conversion can also help database administrators determine if relations should be combined.

### 5. [4.4] What is a Weak Entity Set?

A weak entity set has no primary key and posesses attributes in which some or all belong to another entity set. As a result, the weak entity set has a functional dependency on the strong entity set it is connected, and needs the existence of a related instance within the stong entity.

### 6. [5.2.7; 6.3.8] Explain the concepts of Outerjoin, Natural Right Outer Joins, Natural Left Outer Joins, and Full Outer Joins.

Outerjoin combines rows of two tables while including the unmatched rows from one or both tables, filling the unmatched attributes with null values. Full Outerjoin shows all 3 types of tuples. Left and Right Outerjoin specifies which table should include thier unmatched rows in the outerjoin product.

### 7. [6.6.3] What is the difference between the SQL command `TRANSACTION` and the execution of any statement in SQL?

A transaction allows you to run multiple sql statements at once. The transaction can be started and applied, but needs the COMMIT keyword to save the changes to the databse. It also ensures ACID is upheld for all transactions. The execution of an sql statement does not allow the grouping of multiple transacions and is saved to the database at the time of execution.

### 8. [8] What is a Virtual View and what are its advantages?

A virtual view is a relation that is defined by a query over other relations. This relation is not stored on the database. The view allows the user to update the view without having the changes be applied to all related relations. Another advantage is the concept that the view combines specific values from multiple tables, allowing for easier queries over those values.

### 9. [8.3] What is an *index* and what are its advantages?

An index is a saved attribute/attributes of a relation. An index can speed up the execution of queries or joins focusing on the attribute(s) indexed. This is because the index saves time spent retrieving the data from disk. The use of unique indexes give the advantage of preventing duplicate values in an index.

### 10. Explain the concept of an MVC, or model, view, controller, framework for designing full stack applications

Within an MVC, the model updates or retrieves data from the database and is referred to as the back-end. The view is the front-end user interface used to display data to the user and indicate any changes made to the data. The controller is the median which connects the model to the view. The controller uses input from the front-end to update or display data from the back-end. These three aspects culminate into a full-stack application.

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
