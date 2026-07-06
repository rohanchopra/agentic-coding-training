# AGENTS.md

This project is a beginner-friendly live coding project for building an Amazon sales dashboard with Python and `uv`.

## Project Goals

- Build the dashboard collaboratively during class.
- Keep each step small, understandable, and easy to review.
- Use the Kaggle Amazon Sales Dataset as a local CSV file.
- Practice data loading, cleaning, analysis, visualization, and dashboarding.
- Prefer clear beginner-friendly code over clever abstractions.

## Important Constraints

- Do not commit Kaggle datasets, credentials, API keys, `.env` files, or local auth files.
- Keep downloaded data under `data/raw/` and processed local outputs under `data/processed/`.
- Use `uv` for dependency management and running commands.
- Do not add large frameworks or extra dependencies unless they are needed for the live lesson.
- Make small, reviewable changes that students can understand.
- When asked to explain, do not edit files unless the user clearly asks for changes.

## Expected Commands

Use these patterns when working in the project:

```bash
uv add pandas
uv run python app.py
```

If the project uses Streamlit:

```bash
uv add streamlit plotly
uv run streamlit run app.py
```

## Suggested Structure

The final project may look like this:

```text
student-dashboard/
  README.md
  AGENTS.md
  pyproject.toml
  app.py
  data/
    raw/
      amazon.csv
    processed/
  src/
    student_dashboard/
      __init__.py
      data.py
      charts.py
```

Keep the structure flexible during the lecture. Do not create files before they are useful.

## Data Handling

- Assume the dataset is downloaded manually from Kaggle.
- Do not automate Kaggle login or require Kaggle API credentials unless the instructor asks.
- Load the CSV from `data/raw/amazon.csv` by default.
- If the file is missing, show a clear message explaining where to place it.
- Clean data in small steps and explain each conversion.
- Preserve the raw CSV; write cleaned data only to `data/processed/` if needed.

## Coding Style

- Use plain Python and `pandas` first.
- Keep functions short and named clearly.
- Avoid advanced patterns unless they solve a real problem in the lesson.
- Prefer readable variable names such as `products`, `filtered_products`, and `category_summary`.
- Add comments only when they help beginners understand a non-obvious step.
- Avoid broad rewrites during the live build.

## Dashboard Guidance

- Start with a page title and a small data preview.
- Add metrics before complex charts.
- Add one filter at a time.
- Use charts to answer concrete questions.
- Example question: Which categories have the most products?
- Example question: Which categories have the highest average rating?
- Example question: How are actual price and discounted price related?
- Example question: Which products have the largest discounts?
- Keep the dashboard useful even if some rows have missing or messy values.

## Verification

After code changes, run the smallest relevant check:

```bash
uv run python app.py
```

For Streamlit:

```bash
uv run streamlit run app.py
```

If a command cannot be run because the dataset is missing, report that clearly and do not invent results.

## Collaboration Rules

- Explain what changed and why in beginner-friendly language.
- Ask before making large architecture decisions.
- Do not hide errors; use them as teaching moments.
- When reviewing code, focus on bugs, confusing code, missing checks, and simple improvements.
- Do not overpromise what the dashboard proves; describe findings as observations from this dataset.
