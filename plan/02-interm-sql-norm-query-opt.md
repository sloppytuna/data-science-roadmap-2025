### Phase 2 (6–8 weeks) – Intermediate SQL, normalization, query optimization

**Concepts**

* Normalization in practice (up to 3NF, plus when to denormalize).
* Query patterns:

  * Complex joins.
  * Subqueries, common table expressions (CTEs).
  * Window functions (`ROW_NUMBER`, `RANK`, running totals).
* Indexes: B-tree indexes, composite indexes, when they help.
* Query execution plans (`EXPLAIN`, `EXPLAIN ANALYZE`).
* Transactions, isolation levels (at least conceptually).

**Resources**

* Continue your main SQL course into intermediate topics (the tracks above go this far).([Coursera][2])
* Dip into a classic DB text for theory:

  * **Database System Concepts** (Silberschatz, Korth, Sudarshan) – standard academic reference for relational design, transactions, and internals. ([DB Book][5])

**Project 2: “Public-data analytics DB”**

Pick a sizable public dataset (e.g., NYC 311, taxi data, open real-estate, IMDB, Kaggle). Then:

1. **Model the data**

   * Design a normalized schema.
   * Write DDL to create tables and constraints.
   * Write a simple Python or shell script to load CSVs into Postgres.

2. **Analytics questions**

   * Come up with 10–20 analytics questions that need:

     * Multi-table joins.
     * CTEs.
     * Window functions (e.g., ranking, moving averages).

3. **Performance tuning**

   * Capture baseline query times.
   * Identify slow queries.
   * Add appropriate indexes (and maybe adjust schema).
   * Compare before/after using `EXPLAIN ANALYZE`.

4. **Portfolio packaging**

   * Notebook or markdown file with:

     * The questions.
     * The SQL queries.
     * Commentary on why you indexed what you did and how performance changed.

This is the project that starts to look like “real” analytics/data-science SQL work.