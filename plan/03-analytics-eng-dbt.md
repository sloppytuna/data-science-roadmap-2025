### Phase 3 (4–6 weeks) – Analytics engineering with dbt + a warehouse

Now you move from “one database” to **a small analytics stack**.

**Concepts**

* ELT vs ETL, “modern data stack” architecture.
* Raw → staging → marts modeling pattern.
* Dimensional modeling basics (facts & dimensions).
* Tests, documentation, environments.

**Tools**

* Keep **Postgres** as your “raw” / dev environment.
* Use **dbt Core** as your transformation layer. ([dbt Developer Hub][1])
* Either:

  * Stick with Postgres for everything, or
  * Spin up Snowflake / BigQuery free trial and use dbt’s quickstart for that platform.

**Resources**

* Official dbt **Quickstarts** and intro docs – these are the canonical starting points. ([dbt Developer Hub][6])
* Optionally, DataCamp’s **“Introduction to dbt”** course for a structured walkthrough. ([DataCamp][7])

**Project 3: “Mini warehouse + mart layer”**

Take the public-data project from Phase 2:

1. **Create a dbt project**

   * Connect dbt to your database/warehouse.
   * Create:

     * `raw_` models (or use existing raw tables).
     * `stg_` models: cleaned, standardized.
     * `fct_` and `dim_` models (facts/dimensions).

2. **Add tests & docs**

   * Basic tests: `unique`, `not_null`, simple custom tests.
   * Add column descriptions and run `dbt docs generate`.

3. **Expose**

   * Mark a few key models as “exposures” feeding a BI tool.
   * Point a BI tool (Metabase, Superset, or even Google Data Studio/Looker Studio) at your marts and build 2–3 charts or a small dashboard.

4. **Portfolio packaging**

   * GitHub repo with dbt project.
   * Screenshots/gif of docs site + dashboard.
   * Short writeup: “From raw CSVs to analytics-ready marts in dbt.”

This looks very close to the work of an **analytics engineer / DS with strong SQL**.