# USC DSCI 552 — Homework

Jupyter notebook solutions for DSCI 552 (Machine Learning for Data Science),
instructor Mohammad Reza Rajati.

## Layout

```
.
├── notebook/        # Liu_Yanchen_HW<i>.ipynb — one notebook per assignment
├── midterm/         # Liu_Yanchen_Midterm.ipynb — midterm programming question
├── data/            # datasets + assignment PDFs (gitignored, not committed)
└── requirements.txt # required by the course submission rules
```

Notebooks live in `notebook/` and load data with relative paths such as
`../data/Homework 3, 4 Data/AReM/`. The `data/` directory is gitignored because the
datasets and handouts are distributed by the course, not by this repository.

## Environment

A local virtualenv at `.venv/` (gitignored) holds the dependencies pinned in
`requirements.txt`. Run notebooks with `.venv/bin/python -m jupyter`.

## Rules

@.claude/rules/homework-rule.md
