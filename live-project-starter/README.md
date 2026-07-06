# Amazon Sales Dashboard Live Project

This is the starter guide for the live dashboard project. We will build the app together during the lecture using Python, `uv`, and the Amazon Sales Dataset from Kaggle.

Dataset: <https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset>

## Goal

Build a small dashboard that helps us explore Amazon product sales data.

By the end, the project should be able to:

- Load the Kaggle CSV from a local `data/raw/` folder.
- Inspect and clean the data with Python.
- Show simple summary metrics.
- Add filters for categories, prices, ratings, or discounts.
- Visualize patterns with charts.
- Keep the code understandable enough for beginners to explain.

## Tools

- Python
- `uv` for project setup and dependency management
- `pandas` for data analysis
- A Python dashboard library, chosen during the live build
- An AI coding assistant for pair programming and review

## Before Class

1. Install Python.
2. Install `uv`: <https://docs.astral.sh/uv/getting-started/installation/>
3. Create a Kaggle account if you do not already have one.
4. Open the dataset page: <https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset>
5. Do not commit the dataset file to Git.

## Starting The Project

During the lecture, create a new project folder outside this starter folder:

```bash
uv init student-dashboard --app
cd student-dashboard
```

Add the starter files from this folder to the new project:

```text
README.md
AGENTS.md
```

Then install the libraries selected during the lecture. A likely starting point is:

```bash
uv add pandas
```

If we use Streamlit for the dashboard, we will also run:

```bash
uv add streamlit plotly
```

## Dataset Setup

Download the dataset from Kaggle and place the CSV in this local path:

```text
data/raw/amazon.csv
```

Create a `.gitignore` entry so the downloaded data is not committed:

```gitignore
data/raw/
data/processed/
.env
.venv/
```

## Suggested Project Shape

We may adjust this during the live build.

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
  notebooks/
  src/
    student_dashboard/
      __init__.py
      data.py
      charts.py
```

## Live Build Milestones

1. Create the `uv` project.
2. Add dependencies.
3. Load the CSV with `pandas`.
4. Print the first rows, column names, and data types.
5. Clean column names and convert price, discount, and rating fields if needed.
6. Create basic metrics such as product count, average rating, average discount, and price range.
7. Build a simple dashboard page.
8. Add at least one filter.
9. Add charts for category, rating, price, or discount patterns.
10. Ask the AI assistant to review the code and suggest one small improvement.

## Useful Prompts

Start by asking the assistant to inspect, not edit:

```text
Read this project and explain the files to a beginner. Do not edit files yet.
```

Ask for one small next step:

```text
Add code to load data/raw/amazon.csv with pandas and show the column names. Keep the code beginner-friendly.
```

Ask for help with data cleaning:

```text
Inspect the dataframe columns and suggest the smallest cleaning steps needed before dashboarding. Do not change files yet.
```

Ask for a review:

```text
Review this project for bugs, confusing code, and missing checks. Focus on practical fixes for beginners.
```

## Student Rules

- Make one small change at a time.
- Run the project after each meaningful change.
- Read the diff before accepting AI-generated code.
- Never paste Kaggle credentials, API keys, or secrets into prompts or files.
- Do not commit downloaded data files.
- If code breaks, copy the full error message and ask the assistant to explain it.

## Running The App

The exact command depends on the dashboard library chosen during the lecture.

For a Streamlit app, use:

```bash
uv run streamlit run app.py
```

For a plain Python check, use:

```bash
uv run python app.py
```
