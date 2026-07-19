<div align="center">

# 📸 Instagram Clone Database

### A Relational Database System Modeling a Real-World Social Media Platform

Built with **PostgreSQL**, designed with **proper normalization**, and structured around **real Instagram-like features**.

[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![SQL](https://img.shields.io/badge/SQL-Standard-CC2927?style=for-the-badge&logo=databricks&logoColor=white)](https://en.wikipedia.org/wiki/SQL)
[![Database](https://img.shields.io/badge/Database-Relational-00758F?style=for-the-badge&logo=mysql&logoColor=white)](https://en.wikipedia.org/wiki/Relational_database)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Stars](https://img.shields.io/github/stars/yourusername/instagram-clone-database?style=for-the-badge&color=yellow)](https://github.com/yourusername/instagram-clone-database/stargazers)

</div>

---

## 📖 Overview

**Instagram Clone Database** is a fully normalized relational database that models the core functionality of a social media platform similar to Instagram. It focuses on solid database design fundamentals — entity relationship modeling, normalization up to **BCNF**, and enforced **referential integrity** — rather than application-layer code.

The project includes a complete DDL schema, a realistic sample dataset, and 35+ SQL queries covering everyday CRUD operations as well as complex joins, aggregations, and subqueries. It's designed to demonstrate practical DBMS knowledge applicable to backend, data engineering, and data analysis roles.

---

## ✨ Features Modeled

| Feature | Description |
|---|---|
| 👤 User Accounts | Public, private, business, and creator account types |
| ✅ Verified Accounts | Verification status tracking for eligible users |
| 🖼️ Posts | Multi-media posts (images/videos per post) |
| 🎬 Reels | Short-form video content |
| 📖 Stories & Highlights | Temporary stories with saved highlight collections |
| ❤️ Likes & 💬 Comments | Engagement tracking on posts and reels |
| 🔁 Followers | Many-to-many follow relationships |
| 📩 Direct Messaging | One-to-one and group conversations |
| 📞 Audio/Video Calls | Call logs between users |
| 🌟 Close Friends | Self-referencing relationship for restricted story sharing |
| 🚫 Blocked Users | Self-referencing relationship for user blocking |

---

## 🛠️ Tech Stack

| Category | Technology |
|---|---|
| Database Engine | PostgreSQL |
| Query Language | SQL (DDL, DML, DQL) |
| Design Tools | ER Diagrams, Normalization (BCNF) |
| Documentation | PDF design & normalization reports |

---

## 🧩 Database Design Concepts

- Entity-Relationship (ER) Modeling
- Primary Key & Foreign Key Constraints
- One-to-One Relationships
- One-to-Many Relationships
- Many-to-Many Relationships (via junction tables)
- Self-Referencing Relationships (followers, close friends, blocked users)
- Referential Integrity with `ON DELETE` / `ON UPDATE` rules
- Normalization up to **BCNF** (Boyce-Codd Normal Form)

---

## 📂 Repository Structure

```
instagram-clone-database/
│
├── DDL.sql             # Table definitions, constraints, relationships
├── Data.sql             # Sample dataset for testing and demonstration
├── Queries.sql           # 35+ SQL queries (CRUD, joins, aggregations)
├── Design.pdf            # ER diagram and schema design
├── Normalization.pdf        # Step-by-step BCNF normalization process
└── README.md            # Project documentation
```

---

## ⚙️ Setup Instructions

**1. Clone the repository**
```bash
git clone https://github.com/yourusername/instagram-clone-database.git
cd instagram-clone-database
```

**2. Create a PostgreSQL database**
```sql
CREATE DATABASE instagram_clone;
```

**3. Run the schema**
```bash
psql -U your_username -d instagram_clone -f DDL.sql
```

**4. Load sample data**
```bash
psql -U your_username -d instagram_clone -f Data.sql
```

**5. Run queries**
```bash
psql -U your_username -d instagram_clone -f Queries.sql
```

---

## 🔍 SQL Operations Covered

| Category | Examples |
|---|---|
| Data Retrieval | `SELECT`, `WHERE`, `ORDER BY`, `LIMIT` |
| Joins | `INNER JOIN`, `LEFT JOIN`, self-joins |
| Aggregation | `COUNT`, `SUM`, `AVG`, `GROUP BY`, `HAVING` |
| Subqueries | Correlated and nested subqueries |
| Data Manipulation | `INSERT`, `UPDATE`, `DELETE` |
| Constraints | `PRIMARY KEY`, `FOREIGN KEY`, `UNIQUE`, `CHECK` |

---

## 🎯 Learning Outcomes

- Designing normalized schemas for complex, real-world applications
- Translating business requirements into ER diagrams and relational tables
- Implementing self-referencing relationships for social graph features
- Writing efficient, readable SQL for multi-table queries
- Applying normalization theory (up to BCNF) in a practical setting

---

## 🚀 Future Enhancements

- [ ] Add indexing strategy for query performance optimization
- [ ] Implement stored procedures and triggers for automated actions
- [ ] Add a data analytics layer (views for engagement metrics)
- [ ] Integrate with a backend API (Node.js/Django) for a functional demo

---

## 👨‍💻 Author

**Your Name**
Aspiring Software Engineer | Data Enthusiast

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/yourusername)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/yourusername)

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## ⭐ Support

If you found this project useful or interesting, consider giving it a **star** — it helps others discover it too!

<div align="center">

**Made with 🧠 and a lot of `JOIN`s**

</div>
