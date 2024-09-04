# Database Management - Lab 1

This template repository is the starter project for Database Management Lab 1. Written in Access.

### Question(s)

### Microsoft Access Lab: Tables, Queries, Fields, and Primary Key

#### Objective:
By the end of this lab, students will understand the basic structure of a table, the purpose of fields, how to set a primary key, and how to create and run a query in Microsoft Access.

### Part 1: Creating a Table
#### Step 1: Open Microsoft Access
1. Launch Microsoft Access.
2. Create a new blank database and save it with a name like **StudentRecords.accdb**.

#### Step 2: Create a New Table
1. In the "Table" view, click **Create** > **Table** to open a new table.
2. In the new table, add the following fields:
   - **StudentID** (AutoNumber)
   - **FirstName** (Short Text)
   - **LastName** (Short Text)
   - **DateOfBirth** (Date/Time)
   - **Email** (Short Text)
   - **PhoneNumber** (Short Text)

#### Step 3: Set a Primary Key
1. Right-click the **StudentID** field and select **Primary Key**. This sets **StudentID** as the primary key, ensuring each record is unique.
2. Save the table as **Students** by clicking on the save icon.

#### Questions:
1. What is the purpose of setting a primary key?
2. What data types did you use for each field, and why?

---

### Part 2: Adding Data to the Table
#### Step 1: Enter Data
1. Switch to **Datasheet View** and enter at least five student records.
   - Example:
     - StudentID: Auto-populated
     - FirstName: John
     - LastName: Doe
     - DateOfBirth: 01/15/1998
     - Email: johndoe@example.com
     - PhoneNumber: 555-1234

#### Questions:
1. What do you observe about the **StudentID** field when you enter data?

---

### Part 3: Creating a Query
#### Step 1: Build a Query
1. Go to **Create** > **Query Design**.
2. Select the **Students** table and click **Add**.
3. In the query grid, select the following fields to include in the query:
   - **FirstName**
   - **LastName**
   - **DateOfBirth**
4. In the **Criteria** row for **DateOfBirth**, enter `<= #1/1/2000#`. This will filter students born before January 1, 2000.

#### Step 2: Run the Query
1. Click **Run** on the toolbar to execute the query.
2. The results should display students who were born before the specified date.

#### Questions:
1. What is the purpose of a query in a database?
2. How does using criteria in queries help with filtering data?

---

### Part 4: Modifying the Query
#### Step 1: Add More Criteria
1. In the query grid, add the **Email** field.
2. In the **Criteria** row for **Email**, enter `Like "*example.com"`. This will filter students who have emails ending with "example.com".
3. Run the query again to see the filtered results.

#### Questions:
1. How does the wildcard (`*`) work in the email filtering criteria?
2. Explain how this query helps narrow down information.

---

### Part 5: Conclusion
- **Discussion**: Discuss how tables store raw data, how primary keys help ensure data integrity, and how queries allow users to retrieve specific data based on criteria.
