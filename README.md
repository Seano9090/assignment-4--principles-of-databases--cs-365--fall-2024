# Fall 2024 Principles of Databases — Assignment 4

* **Do not start this project until you’ve read and understood these instructions. If something is not clear, ask.**

---

## ❖ Introduction ❖

For this assignment, you will write responses to nine questions based on different topics from our textbook, *Database Systems — The Complete Book* and to one question based on your notes. Reply to each question in the provided region using Markdown syntax.

---

## ❖ Questions ❖

### 1. [2.4] What is the difference between a Cartesian Product, a Natural Join, and Theta-Joins?

The key difference between cartesian product, a natural join, and theta-joins are as followed. A Cartesian product will return all possible combinations from the tuples. While natural joins combined the tuples only where the common attributes agree. This simplifies queries when attempting to match on shared attributes. While a theta-join will join where a third condition is satisfied. 

### 2. [2.5] What is a Referential Integrity Constraint?

A Referential Integrity Constraint ensures the consistency of the related tables in the database. It will enforce that the rule in one table must correspond to a value inside of the other table. 

###  3. [2.5] What is a Key Constraint?

A key constraint will uniquely identify each tuple in a relation. This is to guarantee no two tuples can have the same value for each specified attribute. The way you implement this would be by assigning a variable name such as "name" assigning the type then following it with 'PRIMARY KEY'.

### 4. [4.1] What is an Entity/Relationship Model? What purpose does it serve in the process of creating/designing databases?

A E/R model is the non visual outline of the database. The purpose is to break down what each entity set will have for attributes and how they make relationships to connect the entity sets. The purpose we make the diagram is to design the graph so we can visualize the database and make it easier to follow as we design it. 

### 5. [4.4] What is a Weak Entity Set?

A weak entity set is when a key is composed of attributes which may overlap via casting an attribute name so when you return the casted attribute you may return the wrong entity. 

### 6. [5.2.7; 6.3.8] Explain the concepts of Outerjoin, Natural Right Outer Joins, Natural Left Outer Joins, and Full Outer Joins.

Outerjoin is when a tuple has dangling attributes that do not have any trace. The reason that the table will append together is to avoid the loss of data but will match the datasets where possible then if not able to will pad it with a null symbol. Natural right outer joins are when the tables are combined and include all rows from the right side and use common names from the columns of both tables. If the rows on the left table don't have a matching value in the right it will null that location. The natural left outer join is the inverse of the natural right outer join. A full outer join is when all rows and columns are combined and then use null where required.
 
### 7. [6.6.3] What is the difference between the SQL command `TRANSACTION` and the execution of any statement in SQL?

Transaction will act as a sentinel waiting for either a COMMIT command which would cause the database to update or a rollback command which would not make any chances to the database leaving it in its original status. It also is either all commands or nothing at all executed. 

### 8. [8] What is a Virtual View and what are its advantages?

A virtual view is a nonreal table that manipulates real tables to allow you to generate results from what is accessed. It acts like a table but will not be able to store data inside of itself. A benefit of a virtual view is the speed in which you can access queries. Ability to shift the views to get the right information that you need to access in some situations. 

### 9. [8.3] What is an *index* and what are its advantages?

An advantage of index’s is the speed that we are able to retrieve data, it works like the index of a book is the best way to explain it. By using where and join conditions we can sort the index structure in order to save time instead of a sorting algorithm. Using this allows us to have access to faster joins, sorting, and functions. 

### 10. Explain the concept of an MVC, or model, view, controller, framework for designing full stack applications

The concept of a MVC or model view controller is very similar to the way that we use a UML language to design a system. This is where we divide the application into subcomponents that interact with each other making complex systems simple. The Model is where the direct interaction with the database comes from and where we can do things such as update, delete, and retrieve data. While the view is where the user is physically able to interact with the application without needing to use a cmd line so anyone can understand how to use the system. The controller is the sentinel which waits for commands from the user and responds with the correct expected results that the user wants to happen. The reason that this is used in a full stack application is because the framework will help the front and backend interact and manage these subcomponents and design tests and different features to ensure the reliability and deployability the application. 

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
