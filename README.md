D-Mart SQL Schema Project
📦 Project Overview
This project is a comprehensive SQL schema design for D-Mart’s Order Management System, simulating real-world retail database operations.
It covers multiple entities like Customers, Orders, Products, Crates, Taxation (HSN), and Order Items with properly defined Primary Keys, Foreign Keys, and Constraints.

The project is designed using Oracle SQL Developer and includes data insertion, table creation, foreign key relationships, and PLSQL elements like joins, exception handling, and transactions.

🗄️ Database Structure
1️⃣ Tables Created:
Table Name	Description
CUSTOMERS	Stores customer details (Name, Contact, Address)
ORDERS	Captures order metadata (Date, Payment Mode, Delivery Time)
ORDER_ITEMS	Detailed product-level information per order
PRODUCTS	List of products with tax categories
HSN_TAX	HSN codes with SGST & CGST details
CRATES	Links orders to specific crate IDs

🔗 Relationships & Constraints
Primary Keys for all tables.

Foreign Keys managing dependencies between:

ORDERS → CUSTOMERS

CRATES → ORDERS

ORDER_ITEMS → CRATES & PRODUCTS

PRODUCTS → HSN_TAX

Referential Integrity maintained across all levels.

⚙️ Features & SQL Concepts Used
DDL (Data Definition Language)
CREATE TABLE, ALTER TABLE, PRIMARY KEY, FOREIGN KEY

DML (Data Manipulation Language)
INSERT INTO with realistic product & order data

PL/SQL Concepts:

Joins (Inner, Left, Right)

Exception Handling

Stored Procedures & Anonymous Blocks (Practiced during development)

Transactions (COMMIT, ROLLBACK)

Indexing & Storage Management handled via Oracle Storage clauses.

🧪 Sample Data
Inserted sample data for Customers, Orders, Crates, Order Items, Products, and HSN tax.

Realistic data simulating a typical D-Mart invoice scenario.

📊 Example Use-Cases
Invoice generation using multi-table joins.

Tax calculation using HSN_TAX linkage.

Order summaries per customer.

Crate management system linked with orders.

🚀 How to Run
Open Oracle SQL Developer or any compatible SQL tool.

Run the dmart_schema.sql file in your workspace.

Ensure you execute INSERT statements after the table creation to populate sample data.

📝 Additional Notes
Developed on: Oracle SQL Developer (Local Setup)

PL/SQL Code (Stored Procedures, Joins, Exception Handling) was practiced during project development for logical testing (not included in raw schema file but part of the learning process).

Normalization Level: 3NF ensured for relational integrity.

📂 Repository Content
File	Description
dmart_schema.sql	Complete DDL and DML SQL file
screenshots/	Sample screenshots of schema & data (captured on mobile and shared via WhatsApp for personal reference)

⚡ Project Status
✅ Completed Core Schema Design
🛠️ Still improving joins, PLSQL procedures, and advanced queries for further optimization.

📎 GitHub Repository
🔗 D-Mart SQL Schema GitHub Repo


Screenshots
<img width="768" height="1024" alt="image" src="https://github.com/user-attachments/assets/2663b4a3-ef53-4ea0-8b4e-991357e52e2c" /> Dmart Bill upon which Schema is made 

<img width="2111" height="594" alt="Screenshot 2025-07-17 184251" src="https://github.com/user-attachments/assets/bc115dd3-996d-4891-8fb8-0352ab549588" />
<img width="2066" height="674" alt="Screenshot 2025-07-17 184259" src="https://github.com/user-attachments/assets/743cef61-9faa-48f8-bde6-28308d9c7fc8" />
<img width="2084" height="685" alt="Screenshot 2025-07-17 184309" src="https://github.com/user-attachments/assets/8d0dc9a5-f356-452a-bfda-25a27ca4880b" />
<img width="2138" height="753" alt="Screenshot 2025-07-17 184318" src="https://github.com/user-attachments/assets/eaeab14b-542b-4847-9261-5c77a6e299bd" />
<img width="2231" height="776" alt="Screenshot 2025-07-17 184327" src="https://github.com/user-attachments/assets/4e036d63-2b46-4150-9a2c-9f19e4424721" />
<img width="2106" height="750" alt="Screenshot 2025-07-17 184333" src="https://github.com/user-attachments/assets/b6a7d7ba-9af9-4e9a-b118-dd2bbc2d8780" />





