## 📘 Week 3 – WorkBook Summary

This section covers my learning outcomes and practical tasks completed during **Week 3** of the **8-week intensive Data Bootcamp** by **Just IT**. The week focused on database fundamentals, relational vs non-relational systems, SQL joins, database schema design, and practical SQL queries using the world database.

---

### 🧩 Database Concepts & Design

Covered essential concepts for designing and understanding relational databases:

- 🔑 **Primary & Foreign Keys**: Ensure uniqueness and table relationships  
- 📚 **1-to-1, 1-to-many, many-to-many** relationships with real-world examples  
- 🧠 **Relational vs Non-relational DBs**:
  - SQL (e.g., MySQL): Structured, schema-based
  - NoSQL (e.g., MongoDB): Flexible, scalable  
- 🏗️ Designed a schema for a retail business (customers, sales, inventory, loyalty)

> ✅ Gained confidence in choosing the right database model based on use case.

---

### 🔧 SQL JOINs – Use Cases & Syntax

| Join Type     | Use Case Example                                             |
|---------------|--------------------------------------------------------------|
| 🔁 Inner Join  | Customers who made purchases                                 |
| ⬅️ Left Join   | All customers, even those without orders                     |
| ➡️ Right Join  | All products, even those never sold                          |
| 🔄 Full Join   | Combine records from both sides, even unmatched              |
| 🔂 Self Join   | Employee-manager hierarchy from the same table               |
| ❎ Cross Join  | Generate all color-size combinations for a product           |

---

### 🏬 Case Study: Retail Business Database Design

Created a relational schema and SQL structure for a local convenience store:

#### Key Tables:
- `Customers`, `Inventory`, `Sales`, `Sale_Items`, `Suppliers`, `Loyalty_Transactions`

#### Database Schema Design:
<p align="center">
  <img src="Pic_Inserted/Retail_Business_Database_Schema.png" width="400" alt="SQL Join Types Overview"/>
</p>

#### Example SQL:
```sql
CREATE TABLE Customers (
  customer_id INT PRIMARY KEY AUTO_INCREMENT,
  first_name VARCHAR(50),
  last_name VARCHAR(50),
  email VARCHAR(100),
  phone VARCHAR(20),
  loyalty_points INT DEFAULT 0
);

---


