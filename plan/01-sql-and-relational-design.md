### Phase 1 (4–6 weeks) – SQL & relational fundamentals

**Concepts**

* Relational model: tables, rows, columns, keys.
* Basic SQL: `SELECT`, `WHERE`, `ORDER BY`, `LIMIT`, `JOIN`, `GROUP BY`, aggregates.
* Constraints: `PRIMARY KEY`, `FOREIGN KEY`, `UNIQUE`, `NOT NULL`.
* Basic normalization: 1NF, 2NF, 3NF.

**Suggested courses (pick one main track)**

* **Track A (Postgres-first, very solid)**:
  *PostgreSQL for Everybody* Specialization (UMich / Coursera) – covers Postgres, SQL, and basic DB design; consistently recommended for serious learners. ([Coursera][2])

* **Track B (DS-flavored)**:
  *SQL Basics for Data Science* Specialization (Coursera) – SQL framed explicitly for data science workloads. ([Mimo][3])

* Supplement with an interactive course if you like: DataCamp’s **“Introduction to SQL”** and follow-up tracks, which are widely used for hands-on SQL practice. ([DataCamp][4])

**Project 1: “Relational Airtable”**

Take a real multi-table Airtable base you use at work or personally (deals, owners, properties, notes, etc.) and:

1. **Design an ER diagram.**

   * List tables + columns.
   * Choose primary keys and foreign keys.
   * Identify one-to-many vs many-to-many relationships (and create junction tables where needed).

2. **Implement the schema in Postgres.**

   * Write `CREATE TABLE` scripts with constraints.
   * Export a subset of Airtable data to CSV and **load via `COPY`** into Postgres.

3. **Replicate “Airtable views” in SQL.**

   * Write queries that mimic:

     * Filtered views (`WHERE`).
     * Grouped rollups (aggregations).
     * Linked records via joins.

4. **Portfolio angle**

   * Put schema + sample queries in GitHub.
   * Write a short README explaining:

     * Original Airtable use case.
     * Pain points.
     * How relational design improves consistency and query power.