# Professional Self-Assessment

## Introduction and Professional Summary

Throughout my academic journey in the Computer Science program, my goal has been to translate theoretical knowledge into practical, real-world solutions. This program has provided a comprehensive foundation in software development, and the capstone project, **Inv-Alert**, serves as the culmination of this learning. As an Android-based inventory management application, Inv-Alert is a testament to my ability to design, build, and deploy a full-stack mobile solution from the ground up.

The skills that I believe set me apart are my focus on creating a secure and user-centric experience. In developing Inv-Alert, I didn't just focus on functionality; I prioritized security principles by implementing password hashing and created an efficient user workflow with features like database-driven sorting. This blend of technical capability and thoughtful design is what I am most proud of and what I believe is essential for a successful career in software engineering. My work on this project, from architecting the SQLite database schema to designing the user interface, demonstrates a readiness to tackle complex challenges and deliver polished, reliable software.

- **Link to the primary project:** [Inv-Alert-Capstone](https://github.com/Jmorgansings/Inv-Alert-Capstone)
- **Link to my ePortfolio narratives:** [CS499 ePortfolio](https://github.com/Jmorgansings/CS499-ePorfolio)

## Meeting Program Learning Outcomes

My work in this course and throughout the program has directly prepared me to meet the core outcomes of the Computer Science curriculum.

---

### **Outcome 1: Software Design and Engineering**

> *"Develop and engineer effective, high-quality, and secure software solutions that meet design specifications and user requirements."*

My entire capstone project is a direct demonstration of this outcome. I engineered a complete software solution based on a clear user need for inventory management.

-   **Artifact:** The `DataDisplayActivity.kt` file within the [Inv-Alert-Capstone](https://github.com/Jmorgansings/Inv-Alert-Capstone/blob/main/app/src/main/java/com/example/jasminemorganinventorymanagement/DataDisplayActivity.kt) project.
-   **Accomplishment:** I applied the **Separation of Concerns** principle by decoupling the UI logic in `DataDisplayActivity.kt` from the data logic in `DatabaseHelper.java`. This creates a maintainable and high-quality codebase. Furthermore, I implemented a "Change Password" feature with secure practices in mind, directly addressing the requirement for secure software.

### **Outcome 2: Algorithms and Data Structures**

> *"Apply fundamental principles of algorithms and data structures to solve complex computational problems."*

The efficiency of my application hinges on the correct application of data structures and algorithmic thinking.

-   **Artifact:** The sorting feature implementation within [DataDisplayActivity.kt](https://github.com/Jmorgansings/Inv-Alert-Capstone/blob/main/app/src/main/java/com/example/jasminemorganinventorymanagement/DataDisplayActivity.kt).
-   **Accomplishment:** Rather than pulling an entire dataset into an `ArrayList` and sorting it in memory (an inefficient approach), I made a deliberate algorithmic choice. I delegated the sorting operation to the SQLite database by constructing a new query with an `ORDER BY` clause. This leverages the database's highly optimized internal algorithms to solve the computational problem of sorting, ensuring the application remains fast and scalable.

### **Outcome 3: Databases**

> *"Design and implement effective database solutions that meet security and performance requirements for a given scenario."*

Data persistence and management are at the core of the Inv-Alert application, and the database was designed to be both robust and efficient.

-   **Artifact:** The [DatabaseHelper.java](https://github.com/Jmorgansings/Inv-Alert-Capstone/blob/main/app/src/main/java/com/example/jasminemorganinventorymanagement/DatabaseHelper.java) class.
-   **Accomplishment:** I designed a relational database schema with `users` and `inventory` tables, ensuring data integrity. I implemented a full suite of CRUD (Create, Read, Update, Delete) methods that encapsulate all SQL logic. The design meets performance requirements by allowing for indexed sorting at the database level and meets security requirements by creating a structure that supports password hashing rather than storing plain text.

### **Outcome 4: Professional Communication**

> *"Communicate professionally and effectively to a variety of audiences about technical concepts and artifacts."*

This ePortfolio itself is the primary artifact for this outcome.

-   **Artifact:** My collection of detailed narratives in the [CS499-ePorfolio](https://github.com/Jmorgansings/CS499-ePorfolio) repository.
-   **Accomplishment:** I have authored three distinct narratives ([Software Design](./software-design.md), [Algorithms & Data Structures](./algorithms-data-structures.md), and [Databases](./databases.md)) that break down complex technical concepts for a varied audience. These documents explain *what* I built and, more importantly, *why* I made specific engineering decisions. This ability to articulate technical work clearly and professionally is a critical skill that I have honed throughout this program.

