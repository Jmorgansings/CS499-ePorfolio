# Software Design and Engineering Narrative

## Artifact Description
**Artifact Link:** [Inv-Alert-Capstone](https://github.com/Jmorgansings/Inv-Alert-Capstone/blob/main/app/src/main/java/com/example/jasminemorganinventorymanagement/DataDisplayActivity.kt)

The primary artifact for demonstrating software design is the `DataDisplayActivity.kt` file. This Kotlin class is the central hub of my inventory management application, responsible for displaying inventory data from a SQLite database, handling user interactions, and implementing key features like sorting and navigation. This activity follows the Single-Responsibility Principle, where its main purpose is to manage the user interface for data presentation. It interacts with a separate `DatabaseHelper` class, decoupling the UI from the data source, which is a fundamental aspect of good software design.

## Design and Engineering Principles

The design of `DataDisplayActivity.kt` was guided by key software engineering principles to ensure the application is robust, maintainable, and user-friendly.

First, I implemented the principle of **Separation of Concerns**. The user interface logic (displaying data in a `RecyclerView`) is contained within this activity, while all database operations (fetching, updating, deleting) are encapsulated within the `DatabaseHelper.java` class. This separation makes the code easier to debug and maintain. For example, if a database query needs to be optimized, I only need to modify `DatabaseHelper.java` without touching the UI code in `DataDisplayActivity.kt`.

Second, I focused on creating a **secure user experience**. The application includes a "Change Password" feature, accessible from the data display screen's menu. This functionality correctly hashes the new password using a salt, preventing plain-text password storage and protecting user credentials, which is a critical security practice.

Finally, the UI was designed for **efficiency and usability**. I implemented a sort feature that allows users to organize the inventory list by product name or quantity. This was achieved by adding a menu to the toolbar and handling the selection events to re-query the database with the appropriate `ORDER BY` clause. This directly addresses a core user need: finding and managing inventory items efficiently. This feature demonstrates my ability to translate user requirements into functional code while maintaining a clean and organized codebase.
