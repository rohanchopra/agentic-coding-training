# Live Project Brief

Build a small data analysis dashboard from a Kaggle dataset.

The dashboard should help students practice asking an AI coding tool to inspect data, create charts, and improve a simple app one step at a time.

This repository should not include the completed dashboard or downloaded Kaggle data. Students will generate their own project during the workshop.

Recommended default for novices: Python, pandas, Streamlit, and Plotly.

Why this stack is a good default:

- The code can stay in one small `app.py` file.
- Students can run the dashboard locally with one command.
- Streamlit gives a dashboard layout without front-end setup.
- pandas and Plotly are common tools for beginner data analysis.

## Requirements

The first version should include only:

- A title.
- A short summary of the chosen Kaggle dataset.
- At least three charts that answer clear questions.
- One small filter or selector.
- A short notes section about missing data, limitations, or assumptions.

## Design

Keep the dashboard readable and simple:

- High-contrast text.
- Clear headings.
- Enough spacing.
- Clear chart titles and axis labels.
- A layout that works well on a laptop screen.

## Starter Prompt

```text
Build the live project described in docs/live-project.md inside a new folder named student-dashboard/. Use Python, pandas, Streamlit, and Plotly. Assume I will download a Kaggle CSV into student-dashboard/data/. Keep the code small enough for beginners to read. After editing, summarize exactly what files changed.
```

After editing, run `streamlit run student-dashboard/app.py`, open the local dashboard in a browser, and review the diff.
