# 🐼 100 Pandas Puzzles — Practice Solutions

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=flat&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> "There are a hundred ways to slice a DataFrame, and roughly ninety-nine of them will trigger a `SettingWithCopyWarning` if you don't know what you're doing."

Welcome to **100 Pandas Puzzles — Practice Solutions**! 🐼

This repository contains my solutions to the well-known [100 Pandas Puzzles](https://github.com/ajcr/100-pandas-puzzles) collection created by Alex Rothberg.

The goal is to develop a deeper understanding of Pandas through hands-on practice, covering everything from basic DataFrame operations and data cleaning to grouping, hierarchical indexing, and time-series analysis.

Rather than simply memorizing syntax, this repository focuses on writing readable, idiomatic Python and understanding the reasoning behind each solution.

Whether you're learning Pandas for the first time or strengthening your data analysis skills, this repository can serve as a practical reference for your journey.

---

## 🧭 Repository Structure & Progress

The solutions are organized into topic-based directories to make learning and revision easier.

| Directory                        | Topic                           | Key Concepts                                                                       |  Status   |
| -------------------------------- | ------------------------------- | ---------------------------------------------------------------------------------- | :-------: |
| `01-dataframe-basics/`           | DataFrame Basics                | Creating DataFrames, `.loc`, `.iloc`, Boolean indexing, column assignment          | 🔄 In Progress |
| `02-data-cleaning/`              | Data Cleaning & Types           | String operations, type conversion, missing values, regular expressions, filtering | ⏳ Pending |
| `03-grouping-and-aggregation/`   | Grouping & Aggregation          | `.groupby()`, `.agg()`, cumulative sums, ranking, transformations                  | ⏳ Pending |
| `04-multi-indexing-and-slicing/` | MultiIndex & Slicing            | Hierarchical indexing, tuple-based slicing, `.xs()`, swapping levels, `unstack()`  | ⏳ Pending |
| `05-window-and-time/`            | Time Series & Window Operations | Rolling windows, `.shift()`, datetime conversion, frequency offsets                | ⏳ Pending |

*Directory names, topics, and completion statuses will be updated as work progresses.*

---

## 💡 How to Use This Repository

The objective is not just to obtain the correct output. It is to understand why a solution works and how to write better Pandas code.

1. **Attempt the problem first.** Read the original puzzle and spend around 15 minutes developing your own solution in Python or Jupyter Notebook.
2. **Think in terms of operations on entire columns.** Before using explicit row-by-row loops, consider whether Pandas provides a vectorized operation.
3. **Compare your approach.** Review the corresponding solution and identify differences in readability, efficiency, and correctness.
4. **Understand the reasoning.** Pay attention to indexing, data types, missing values, and other edge cases.
5. **Experiment with alternatives.** Modify the input data and test whether your solution behaves as expected.

The goal is to build practical skills that transfer to real-world data analysis, not merely to finish 100 puzzles.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
# Clone the repository
git clone https://github.com/tninanofchirawa/ds-puzzles-and-exercises.git

# Navigate to the 100 Pandas Puzzles
cd ds-puzzles-and-exercises/03-pandas-puzzles-100
```

### 2. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate the environment:

**Windows — Command Prompt**

```bash
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

If the repository contains a `requirements.txt` file, install the dependencies using:

```bash
python -m pip install -r requirements.txt
```

Otherwise, install Pandas directly:

```bash
python -m pip install pandas
```

### 4. Run the Solutions

Open the relevant Python script or notebook in your preferred editor and run it using your Python environment.

---

## 📚 Curated Learning Resources

Solving puzzles is useful, but understanding the underlying concepts makes the learning process much more effective. The following resources complement the exercises.

### 🎓 University Courses & Lecture Materials

- [UC Berkeley Data 100 — Principles and Techniques of Data Science](https://ds100.org/)  
  A university-level introduction to data science, data manipulation, relational operations, and analytical workflows.

- [Harvard CS109A — Introduction to Data Science](https://harvard-cs109.github.io/2021-CS109A/)  
  Course materials and notebooks covering foundational data science concepts and practical Python workflows.

### 🐙 GitHub Repositories

- [wesm/pydata-book](https://github.com/wesm/pydata-book)  
  Companion notebooks for _Python for Data Analysis_ by Wes McKinney, the creator of Pandas.

- [TomAugspurger/effective-pandas](https://github.com/TomAugspurger/effective-pandas)  
  Examples and materials focused on idiomatic Pandas, method chaining, and maintainable data transformations.

### 📖 Books & Official Documentation

- [Python Data Science Handbook — Jake VanderPlas](https://jakevdp.github.io/PythonDataScienceHandbook/)  
  A free online book covering NumPy, Pandas, data visualization, and machine learning fundamentals.

- [Pandas Official Documentation](https://pandas.pydata.org/docs/user_guide/index.html)  
  The official user guide, with explanations and examples of indexing, data selection, missing data, grouping, reshaping, and time-series functionality.

- [Effective Pandas — Matt Harrison](https://store.metasnake.com/effective-pandas-book)  
  A practical resource for writing clear, maintainable, and efficient Pandas code.

### 🎥 Video Tutorials

- [Pandas Full Course — freeCodeCamp](https://www.youtube.com/watch?v=vmEHCJofslg)  
  A comprehensive introduction to working with tabular data using Pandas.

- [Corey Schafer — Pandas Tutorials](https://www.youtube.com/watch?v=ZyhVh-qRZPA&list=PL-osiE80TeTsWRelO5q5oOxEkAK5-KGvv)  
  Step-by-step tutorials covering data selection, filtering, grouping, and cleaning.

- [Rob Mulla — Exploratory Data Analysis with Pandas](https://www.youtube.com/watch?v=xi0vhXFPegA)  
  A practical demonstration of exploratory data analysis and data-wrangling techniques.

- [Data School — Pandas Best Practices](https://www.youtube.com/watch?v=dPwLlJkSHLo)  
  Practical advice on common Pandas operations, mistakes, and effective workflows.

---

## 🎯 Learning Objectives

Through these exercises, the repository aims to strengthen the following skills:

- **Data manipulation:** Create, select, filter, and transform DataFrames.
- **Data cleaning:** Handle missing values, inconsistent types, and messy strings.
- **Aggregation:** Summarize datasets using grouping, ranking, and transformation operations.
- **Advanced indexing:** Work confidently with MultiIndex objects and complex selections.
- **Time-series analysis:** Apply datetime conversion, shifting, and rolling-window operations.
- **Code quality:** Write readable, maintainable, and appropriately vectorized Pandas solutions.
- **Independent problem-solving:** Develop the habit of understanding a problem before searching for an implementation.

These skills provide a foundation for exploratory data analysis, statistical computing, and machine learning workflows.

---

## ⚖️ Attribution & License

### Original Puzzle Collection

The exercises are based on [100 Pandas Puzzles](https://github.com/ajcr/100-pandas-puzzles), created by Alex Rothberg ([@ajcr](https://github.com/ajcr)). Credit for the original puzzle collection belongs to its author.

### My Contributions

This repository contains my practice solutions, implementation choices, comments, and explanations. The solutions are intended for learning, experimentation, and reference.

### License

This repository is distributed under the **MIT License**, provided that the repository includes an appropriate `LICENSE` file and that the licensing and attribution requirements applicable to the original materials are respected.

See the [`LICENSE`](https://github.com/ajcr/100-pandas-puzzles/blob/master/LICENSE) file for the license governing this repository.

---

## 🙌 Final Note

One puzzle at a time. One concept at a time. One better solution at a time.

The aim is not just to make Pandas work, but to understand it well enough to use it confidently in real data science projects.

**Happy coding! 🐼🐍**
