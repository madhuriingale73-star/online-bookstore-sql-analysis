# Online Bookstore Data Analytics Project (SQL)

## Project Overview
This project focuses on building a relational database schema for an **Online Bookstore** platform and extracting actionable business insights using **PostgreSQL**. The dataset consists of three key entities: Books, Customers, and Orders. Through a series of basic to advanced SQL queries, we analyze inventory health, revenue generation, and customer purchase behaviors.

## Database Architecture
The database schema consists of three core tables linked via relational constraints:
* **Books**: Stores book attributes including pricing, genre, and real-time inventory counts.
* **Customers**: Manages customer demographic details (City, Country).
* **Orders**: Connects customers to their purchased books, capturing transaction dates and volume.

### Relational Schema Diagram
- `Books.Book_ID` ─── < Primary Key / Foreign Key > ─── `Orders.Book_ID`
- `Customers.Customer_ID` ─── < Primary Key / Foreign Key > ─── `Orders.Customer_ID`

## Project Questions Resolved

### Basic Business Questions
1. Retrieve all books belonging to the "Fiction" genre.
2. Find books published after the year 1950.
3. List all customers residing in Canada.
4. Show all orders placed specifically in November 2023.
5. Retrieve the total stock of books available across the inventory.
6. Extract the complete details of the most expensive book.
7. Show all customers who purchased more than 1 quantity of any book.
8. Retrieve all orders where the total transactional amount exceeds \$20.
9. List all unique genres available in the database.
10. Find the book holding the lowest remaining stock.
11. Calculate the total aggregate revenue generated from all orders.

### Advanced Analytical Insights
1. Extract the total number of books sold, broken down by individual genre.
2. Find the average price of books categorized under the "Fantasy" genre.
3. List high-value customers who have placed 2 or more distinct orders.
4. Find the most frequently ordered book title.
5. Show the top 3 most expensive books within the 'Fantasy' genre.
6. Calculate the total cumulative quantity of books sold by each author.
7. List distinct cities where customers who spent over \$30 on a single order are located.
8. Identify the single customer who has spent the most total money across all orders.
9. Calculate remaining inventory stock metrics dynamically after fulfilling all customer orders.

## Technologies Used
* **Database Engine:** PostgreSQL
* **Tooling:** pgAdmin / SQL Command Line (`psql`)
* **Format:** Raw CSV Data Datasets

## How to Run This Project
1. Clone this repository to your local drive.
2. Open your PostgreSQL terminal or tool.
3. Execute the schema script located at `scripts/database_setup.sql` to initialize your tables and database.
4. Import the structured CSV files found within the `data/` directory.
5. Execute the query collection in `scripts/analytics_queries.sql` to extract the analytics findings.
