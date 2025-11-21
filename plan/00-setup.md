### Phase 0 (1–2 weeks) – Setup & bridge from Airtable

**Goals**

* Install tooling.
* Translate your Airtable mental model to classic relational ideas.

**Do**

* Install **PostgreSQL** locally (or via Docker) + a GUI (DBeaver / TablePlus).
* Set up **Git** and create a **“sql-playground”** repo on GitHub.
* Read a short intro to relational DBs & SQL (any tutorial; a few chapters from a SQL course).

**Mini-project: “Hello, Deals DB”**

* Take a small Airtable base you know (e.g., deals + contacts).
* Sketch entities: `deals`, `owners`, `properties`, `contacts`.
* Create tables in Postgres with primary keys + foreign keys.
* Insert a few rows manually via `INSERT` to get comfortable with the workflow.