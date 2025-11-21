### Phase 4 (6–12+ weeks) – End-to-end data-science workflows

Now you integrate **Python + modeling** with the stack you’ve built.

**Concepts**

* Using SQL as a **feature-engineering / data-prep layer**.
* Pulling features into Python (Pandas, scikit-learn).
* Basic ML workflow: train/test split, cross-validation, evaluation metrics.
* Reproducibility: notebooks + scripts + config.

**Minimal Python stack**

* Python 3.x, virtualenv/poetry or conda.
* Libraries: `pandas`, `numpy`, `sqlalchemy` or `psycopg2`, `scikit-learn`, `matplotlib` or `plotly`.

**Project 4: “Full pipeline DS project”**

Pick a problem where you can plausibly tell a story to a hiring manager (e.g., predicting building lease-up speed, property churn, simple pricing model, customer churn in some open dataset).

1. **Data layer**

   * Ingest raw data into Postgres.
   * Use dbt to transform into clean feature tables.

2. **Modeling layer (Python)**

   * Write a notebook that:

     * Queries dbt models via SQL.
     * Does minimal extra feature work in Pandas.
     * Trains a baseline model (logistic or linear regression, maybe a tree-based method).
     * Evaluates performance and visualizes key results.

3. **Reproducibility**

   * Factor reusable code into `.py` modules.
   * Include a `requirements.txt` or `pyproject.toml`.
   * Document how to run: “From raw data to trained model in N steps.”

4. **Portfolio packaging**

   * GitHub repo with:

     * `dbt` folder.
     * `notebooks/`.
     * `src/` for scripts.
   * A short **project report** (Markdown or PDF) summarizing:

     * Business question.
     * Data model and pipeline.
     * Model approach and results.
     * Limitations & next steps.