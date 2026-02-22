College Database Design (DB Lab)

**Overview**

This project demonstrates the design and implementation of a College Database System using the Entity-Relationship (ER) model and SQL.
The database manages departments, students, faculty members, courses, and course enrollments.

The assignment includes:

- ER Diagram
- Conversion to relational tables
- SQL implementation using "CREATE TABLE"

---

**Entities**

Department

Stores information about academic departments in the college.

**Attributes:**

- Department_ID (Primary Key)
- Department_Name
- Office_Location

---

**Student**

Contains details of students enrolled in the college.

Attributes:

- Student_ID (Primary Key)
- Name
- Date_of_Birth
- Gender
- Contact_Number
- Department_ID (Foreign Key)

Relationship:

- A student belongs to one department.
- A student can enroll in multiple courses.

---

Faculty

Stores details of faculty members.

Attributes:

- Faculty_ID (Primary Key)
- Name
- Designation
- Email
- Department_ID (Foreign Key)

Relationship:

- A faculty member works in one department.
- A faculty member can teach multiple courses.

---

**Course**

Represents subjects offered by departments.

Attributes:

- Course_ID (Primary Key)
- Course_Name
- Credits
- Department_ID (Foreign Key)
- Faculty_ID (Foreign Key)

Relationship:

- A course belongs to one department.
- A course is taught by one faculty member.

---

Enrollment

Handles the many-to-many relationship between students and courses.

Attributes:

- Student_ID (Primary Key, Foreign Key)
- Course_ID (Primary Key, Foreign Key)
- Semester
- Grade

---

Relationships

Entity| Relationship| Entity| Type
Department| has| Students| One to Many
Department| has| Faculty| One to Many
Department| offers| Courses| One to Many
Faculty| teaches| Course| One to Many
Student| enrolls in| Course| Many to Many

---

**Database Tables**

1. Department
2. Student
3. Faculty
4. Course
5. Enrollment

Each table is connected using Primary Keys and Foreign Keys.

---

**SQL Implementation**

The database schema is implemented using SQL "CREATE TABLE" statements with:

- Appropriate data types
- Primary Key constraints
- Foreign Key constraints
- Composite key for Enrollment table

---

**Tools Used**

- Draw.io / Diagrams.net for ER Diagram
- MySQL / SQL environment
- GitHub for submission

---

**Learning Outcome**

Through this assignment we learned:

- Entity Relationship Modeling
- Database Normalization basics
- Table relationships
- SQL table creation
- Use of primary and foreign keys

---



DB Lab Assignment
College Database Project
