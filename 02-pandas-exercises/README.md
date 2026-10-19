# 📊 Pandas Real-World Exercises — Practice Solutions

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=flat&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> *"Synthetic toy data is polite. Real-world data arrives with unparsed timestamps, corrupted numbers disguised as strings, missing values, and inconsistent records — just to see if you're paying attention."*

Welcome to **Pandas Real-World Exercises — Practice Solutions!** 📊

This repository contains my solutions to practical data manipulation exercises inspired by the [Pandas Exercises](https://github.com/guipsamora/pandas_exercises) collection.

Instead of focusing exclusively on isolated examples, these exercises explore realistic data-analysis workflows involving filtering, grouping, merging, time-series processing, statistical summaries, and exploratory data analysis.

Working with datasets such as restaurant orders, international sporting results, alcohol consumption statistics, and other real-world examples helps develop the skills needed to transform raw data into meaningful insights.

The focus is on writing readable, maintainable Python code and understanding the reasoning behind each data transformation.

---

## 🧭 Topic Structure & Progress

The repository is organized into topic-based directories to make individual exercises easier to find, understand, and revisit.

| Directory | Topic | Key Operations & Concepts | Status |
|---|---|---|:---:|
| `01-filtering-and-sorting/` | Filtering & Sorting | Boolean indexing, `.loc`, `.query()`, `.sort_values()`, conditional selection | 🔄 In Progress |
| `02-grouping/` | Grouping & Aggregation | `.groupby()`, `.agg()`, `.transform()`, custom aggregations, multi-column grouping | ⏳ Pending |
| `03-merge-and-joins/` | Merging & Combining Data | `pd.merge()`, join types, merge indicators, `pd.concat()`, index alignment | ⏳ Pending |
| `04-time-series/` | Time-Series Analysis | Datetime conversion, `.resample()`, rolling windows, time-based indexing | ⏳ Pending |
| `05-stats-and-visualization/` | Statistics & Exploratory Data Analysis | Descriptive statistics, quantiles, `.describe()`, correlations, visualizations | ⏳ Pending |

*Directory names, topics, and completion statuses will be updated as work progresses.*

---

## 💡 Practical Rules for Working with Real Data

Real-world data analysis requires more than knowing which Pandas method to call. It also requires careful decisions about data quality, correctness, and maintainability.

1. **Clean data early.** Inspect column types, missing values, inconsistent strings, and malformed dates before performing complex transformations. Use appropriate conversion and validation methods rather than assuming the input is clean.

2. **Chain responsibly.** Methods such as `.assign()`, `.query()`, and `.pipe()` can make transformations easier to follow. However, split complicated workflows into meaningful steps when doing so improves debugging and readability.

3. **Handle data types explicitly.** Inspect columns with `.dtypes` and `.info()`. Use appropriate conversions, such as `pd.to_numeric()` and `pd.to_datetime()`, while deciding how invalid values should be handled.

4. **Treat missing values deliberately.** Understand how `NaN`, `None`, and `NaT` affect filtering, aggregation, and calculations. Choose whether to remove, preserve, or impute missing values based on the problem.

5. **Validate merges and joins.** Check key uniqueness, unexpected unmatched records, and duplicate rows. Use merge validation and indicator columns when appropriate.

6. **Avoid unnecessary row-by-row processing.** Prefer vectorized operations when they express the intended calculation clearly and efficiently. Use explicit iteration when it is genuinely needed.

7. **Check your results.** Validate shapes, data types, row counts, and summary statistics after important transformations. A script running without errors does not necessarily mean the analysis is correct.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
# Clone the repository
git clone https://github.com/tninanofchirawa/ds-puzzles-and-exercises.git

# Navigate to the Pandas exercises
cd ds-puzzles-and-exercises/02-pandas-exercises
```

### 2. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate it using the appropriate command for your operating system.

**Windows — Command Prompt**

```bat
.venv\Scripts\activate
```

**Windows — PowerShell**

```powershell
.\.venv\Scripts\Activate.ps1
```

**Linux / macOS**

```bash
source .venv/bin/activate
```

### 3. Install Dependencies

If the repository contains a `requirements.txt` file, run:

```bash
python -m pip install -r requirements.txt
```

Otherwise, install the essential packages directly:

```bash
python -m pip install pandas numpy matplotlib
```

Install additional libraries only if the exercises require them.

### 4. Explore the Exercises

Open the relevant Python script or Jupyter Notebook in your preferred development environment.

For each exercise, try to understand:

- What the raw dataset contains.
- What transformation or analytical question is required.
- Why a particular Pandas operation is appropriate.
- How to verify that the result is correct.

---

## 📚 Curated Learning Resources

These resources complement the exercises by explaining the concepts behind practical data manipulation and analysis.

### 🎓 University Courses & Lecture Materials

- [UC Berkeley Data 100 — Principles and Techniques of Data Science](https://ds100.org/)  
  Course materials covering data manipulation, relational operations, data cleaning, and analytical workflows.

- [NYU Data Bootcamp](https://nyudatabootcamp.github.io/)  
  Practical materials focused on data analysis, visualization, and working with economic and financial datasets.

### 🐙 GitHub Repositories

- [wesm/pydata-book](https://github.com/wesm/pydata-book)  
  Companion code and notebooks for *Python for Data Analysis* by Wes McKinney.

- [justmarkham/pandas-videos](https://github.com/justmarkham/pandas-videos)  
  Code examples and supporting materials for learning Pandas through practical demonstrations.

- [guipsamora/pandas_exercises](https://github.com/guipsamora/pandas_exercises)  
  The original exercise collection that inspires this repository's practical approach to learning Pandas.

### 📖 Books & Essential Reading

- [Python Data Science Handbook — Jake VanderPlas](https://jakevdp.github.io/PythonDataScienceHandbook/)  
  A free online book introducing NumPy, Pandas, data visualization, and machine learning fundamentals.

- [Pandas Official User Guide](https://pandas.pydata.org/docs/user_guide/index.html)  
  The official reference for indexing, missing data, grouping, merging, reshaping, and time-series operations.

- [Tidy Data — Hadley Wickham](https://vita.had.co.nz/papers/tidy-data.pdf)  
  An influential paper explaining principles for structuring datasets to simplify analysis.

### 🎥 Video Tutorials & Practical Walkthroughs

- [Data School — Selecting a Subset of a DataFrame](https://www.youtube.com/watch?v=2AFGPdNn4EE)  
  A practical introduction to selecting rows and columns using Pandas indexing techniques.

- [Rob Mulla — Exploratory Data Analysis with Pandas](https://www.youtube.com/watch?v=xi0vhXFPegA)  
  A hands-on walkthrough of exploratory analysis and data-wrangling techniques.

- [Keith Galli — Sales Data Analysis with Python](https://www.youtube.com/watch?v=eMOA1pPVUc4)  
  A practical example of analyzing transactional sales data using Python.

- [Brandon Rhodes — Pandas from the Ground Up](https://www.youtube.com/watch?v=5JnMutdy6Fw)  
  A conceptual introduction to Pandas, including indexing and data manipulation.

---

## 🎯 Learning Objectives

By completing these exercises, the repository aims to strengthen the following skills:

- **Data filtering:** Select relevant records using conditions and Boolean indexing.
- **Data cleaning:** Handle missing values, inconsistent formats, and incorrect data types.
- **Grouping and aggregation:** Summarize datasets and compare groups using appropriate statistical operations.
- **Relational operations:** Combine datasets through joins, merges, and concatenation.
- **Time-series analysis:** Work with timestamps, time-based indexes, resampling, and rolling calculations.
- **Exploratory data analysis:** Investigate distributions, relationships, trends, and potential anomalies.
- **Code quality:** Write readable, maintainable, and appropriately vectorized Pandas workflows.
- **Data validation:** Check assumptions and verify results before drawing conclusions.

These skills form an important foundation for data science, statistical analysis, reporting, and machine learning.

---

## ⚖️ Attribution & License

### Original Exercise Collection

This repository is inspired by [Pandas Exercises](https://github.com/guipsamora/pandas_exercises), associated with Guilherme Samora ([@guipsamora](https://github.com/guipsamora)) and contributors.

Credit for the original exercises and any reused materials belongs to their respective authors.

### My Contributions

This repository contains my practice implementations, original explanations, and analytical workflows developed while working through the exercises.

### License

This repository is intended to be distributed under the **MIT License**, subject to the actual contents of its `LICENSE` file and any applicable licensing requirements for reused material.

See [`LICENSE`]([LICENSE](https://github.com/guipsamora/pandas_exercises/blob/master/LICENSE)) for the license governing this repository. Verify the upstream project's license before redistributing its exercises, datasets, or other materials.

---

## 🙌 Final Note

Real-world data is rarely perfect. Learning to work with it requires patience, careful reasoning, and a willingness to investigate unexpected results.

One dataset at a time. One transformation at a time. One insight at a time.

**Happy data wrangling! 📊🐍**
