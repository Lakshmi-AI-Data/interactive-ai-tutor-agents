# Project Creation Helper (Use ONLY when Project 1 begins)

**Do not read this section until your tutor says: “Project 1 begins.”**  
This guide helps you set up FREE tools, load a Kaggle dataset, and publish your project on GitHub.

---

## A) Free tools (choose ONE path)

### Path 1 (Recommended for beginners): SQLite + DB Browser
- DB Browser for SQLite (downloads): https://sqlitebrowser.org/dl/ 
- SQLite official downloads (optional): https://www.sqlite.org/download.html 

### Path 2 (Also good): DBeaver Community (supports many databases, incl. SQLite)
- DBeaver download: https://dbeaver.io/download/ 

### Optional IDE (for writing .sql neatly)
- VS Code download: https://code.visualstudio.com/download 

> If you are on Linux, avoid installing VS Code via Snap if possible (there are known issues).

---

## B) Create your GitHub account + repository

### Step B1: Create a GitHub account
Follow GitHub’s official guide:  
- Creating an account on GitHub: https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github

### Step B2: Create a new repository
GitHub “Quickstart for repositories”:  
https://docs.github.com/en/repositories/creating-and-managing-repositories/quickstart-for-repositories

**Repository naming examples**
- `sql-project-student-performance`
- `sql-project-ecommerce-sales`
- `sql-project-public-health`

**Visibility**
- Public is recommended (recruiters can see it).

---

## C) Standard project folder structure (copy exactly)
Create these folders in your repo:

```
README.md
data/
schema/
queries/
outputs/
notes/
```

**What goes where**
- `data/` : Kaggle CSV (or small sample)
- `schema/` : CREATE TABLE scripts
- `queries/` : your analysis queries (commented)
- `outputs/` : screenshots of charts + sample results
- `notes/` : learning notes + progress snippets

---

## D) Pick a dataset (Kaggle suggested)
Your tutor will help you pick a dataset. Common beginner-friendly options:
- Student performance / marks / attendance (Academic)
- Online retail / e-commerce sales (Business)
- Public health / vaccination / survey (Social impact)

---

## E) Load the CSV into your database (SQLite example)
### Step E1: Create a database
Create: `project1.db`

### Step E2: Create tables
Put your CREATE TABLE scripts in:
- `schema/create_tables.sql`

### Step E3: Import CSV
Using DB Browser or DBeaver:
- Import CSV into the correct table(s)
- Verify columns match

### Step E4: Validate after loading
Run these checks:
1. Row counts: do they match the CSV?
2. Null checks: are keys missing (IDs)?
3. Range checks: marks/revenue within sensible limits
4. Duplicates: duplicate IDs where not expected

Document what you checked in:
- `notes/data_validation.md`

---

## F) Write required deliverables (Project 1)
Project 1 must include:

### SQL
- 15–25 queries total
- Every query has a short comment describing the business question

Suggested files:
- `queries/01_basic_filters.sql`
- `queries/02_aggregations.sql`
- `queries/03_quality_checks.sql`
- `queries/04_insights.sql`

### Insights
- 5+ insights written in plain English
Add to `README.md` under “Insights”.

### Visuals (required)
- 2–4 basic charts (Excel/Sheets is fine)
Examples:
- Top 5 categories by revenue
- Department average marks
- Trend by month/term

Save screenshots in:
- `outputs/charts/`

---

## G) Push to GitHub (two ways)

### Option 1 (easiest): Upload via GitHub website
- Repo → **Add file** → **Upload files** → Commit changes

### Option 2 (recommended): Use Git on your computer
If you already have Git installed:
- Clone the repo
- Add files
- Commit + push

(Your tutor can guide you step-by-step if needed.)

---

## H) README template (copy/paste)
In `README.md`, include:

1. Project title  
2. Problem statement  
3. Dataset source (Kaggle link)  
4. Schema overview (tables + purpose)  
5. How to run (tool + steps)  
6. Key queries (short list)  
7. Insights (5+)  
8. Charts (screenshots)  
9. What you learned

---

## Done Definition (what “complete” looks like)
- Repo has the folder structure
- SQL scripts are readable and commented
- 15–25 meaningful queries
- 5+ insights
- 2–4 charts in outputs
- README is clear and reproducible
