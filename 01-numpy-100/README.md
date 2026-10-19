# ⚡ 100 NumPy Exercises — Handwritten Solutions

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![NumPy](https://img.shields.io/badge/NumPy-013243.svg?style=flat&logo=numpy&logoColor=white)](https://numpy.org/)
[![License: BSD-3-Clause](https://img.shields.io/badge/License-BSD--3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)

> *"Life is too short to write nested Python loops over multidimensional arrays. Learn to think in arrays, embrace vectorization, and let NumPy do the heavy lifting."*

Welcome to **100 NumPy Exercises — Handwritten Solutions!** ⚡

This repository contains my solutions to the [100 NumPy Exercises](https://github.com/rougier/numpy-100) collection, an exercise set designed to develop practical proficiency with NumPy.

From basic array creation and indexing to broadcasting, linear algebra, and advanced array manipulation, these exercises provide an opportunity to understand how NumPy works and how to use it effectively.

The focus is on writing clear, idiomatic Python, understanding array operations, and developing a stronger foundation for scientific computing, numerical analysis, data science, and machine learning.

---

## 🧭 Repository Structure & Progress

The solutions are organized into topic-based directories for easier navigation and revision.

| Directory | Core Topics | Key Operations & Concepts | Status |
|---|---|---|:---:|
| `01-vectors-and-matrices/` | Vectors & Basic Matrices | Array creation, `zeros()`, `ones()`, `arange()`, slicing, Boolean indexing | 🔄 In Progress |
| `02-array-manipulation/` | Reshaping & Broadcasting | `reshape()`, `newaxis`, broadcasting, transposition, flattening, views | ⏳ Pending |
| `03-linear-algebra-and-ops/` | Linear Algebra & Vectorization | Dot products, inner and outer products, matrix operations, `np.linalg`, norms, eigenvalues | ⏳ Pending |
| `04-advanced-and-miscellaneous/` | Advanced Arrays & Memory Layouts | Strides, structured arrays, universal functions, byte order, advanced indexing | ⏳ Pending |

*Update the directory names and completion statuses to reflect the actual contents of your repository.*

---

## 💡 How to Approach These Puzzles

The objective is not simply to obtain the correct output. It is to understand how NumPy represents and manipulates numerical data.

1. **Think in arrays.** Before writing an explicit Python loop, consider whether a vectorized NumPy operation can express the same computation more clearly. Loops are not inherently wrong, but array operations are often more concise and can be substantially faster.
2. **Understand views and copies.** Array slicing may produce a view that shares memory with the original array, while some indexing operations create copies. Know the difference before modifying an array.
3. **Master broadcasting.** Learn how NumPy aligns dimensions from right to left and when dimensions are compatible for element-wise operations.
4. **Pay attention to shapes.** Check array dimensions, axes, and data types whenever an operation produces an unexpected result.
5. **Explore memory layout.** Understand the relationship between shape, strides, contiguity, and views to make better decisions when working with large arrays.
6. **Experiment with alternatives.** Compare implementations for readability, correctness, and performance instead of assuming that a shorter expression is always faster.

The goal is to develop an array-oriented way of thinking that transfers to larger scientific computing and data science problems.

---

## 🚀 Getting Started

### 1. Clone the Repository

Replace `<your-username>` with your GitHub username.

```bash
git clone https://github.com/tninanofchirawa/ds-puzzles-and-exercises.git
cd numpy-100-solutions
```

### 2. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate it using the command for your operating system.

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

If the repository contains a `requirements.txt` file:

```bash
python -m pip install -r requirements.txt
```

Otherwise, install NumPy directly:

```bash
python -m pip install numpy
```

### 4. Run the Solutions

Open a Python script or Jupyter Notebook from the relevant directory and execute the exercises in your preferred development environment.

---

## 📚 Curated Learning Resources

Don't just memorize functions. Build a strong mental model of arrays, broadcasting, numerical computation, and memory layout.

### 🎓 University Lectures & Course Materials

- [Stanford CS231n — Python and NumPy Tutorial](https://cs231n.github.io/python-numpy-tutorial/)  
  A practical introduction to Python, NumPy arrays, indexing, and vectorized numerical operations.

- [SciPy Lecture Notes](https://scipy-lectures.org/)  
  Educational materials covering scientific Python, NumPy, array manipulation, and numerical computing.

### 🐙 GitHub Repositories

- [rougier/from-python-to-numpy](https://github.com/rougier/from-python-to-numpy)  
  Nicolas P. Rougier's open-source book exploring vectorization and the transition from ordinary Python code to efficient NumPy operations.

- [scipy-lectures/scipy-lecture-notes](https://github.com/scipy-lectures/scipy-lecture-notes)  
  Source materials for a comprehensive introduction to the scientific Python ecosystem.

### 📖 Books & Official Documentation

- [From Python to NumPy — Nicolas P. Rougier](https://www.labri.fr/perso/nrougier/from-python-to-numpy/)  
  A free online resource for understanding vectorized computation and array-oriented programming.

- [NumPy User Guide](https://numpy.org/doc/stable/user/index.html)  
  The official documentation covering array creation, indexing, broadcasting, data types, and other fundamental concepts.

- [Python Data Science Handbook — Jake VanderPlas](https://jakevdp.github.io/PythonDataScienceHandbook/)  
  A free online book introducing NumPy, Pandas, data visualization, and machine learning. Chapter 2 focuses on NumPy.

### 🎥 Video Tutorials & Technical Talks

- [NumPy Full Course — freeCodeCamp](https://www.youtube.com/watch?v=QUT1VHiLmmI)  
  A practical introduction to arrays, indexing, mathematical operations, and statistics.

- [Keith Galli — Complete NumPy Tutorial](https://www.youtube.com/watch?v=GB9BytCEH8Y)  
  A hands-on walkthrough of NumPy fundamentals and common array operations.

- [Jake VanderPlas — Losing Your Loops](https://www.youtube.com/watch?v=EEUXKG97YRw)  
  A technical talk on vectorization and improving numerical computing workflows with NumPy.

---

## 🎯 Learning Objectives

By working through these exercises, the repository aims to strengthen the following skills:

- **Array fundamentals:** Create, initialize, inspect, and manipulate multidimensional arrays.
- **Indexing and slicing:** Select elements, construct masks, and access specific regions of an array.
- **Broadcasting:** Perform operations across compatible array dimensions without manually repeating data.
- **Vectorization:** Express numerical computations through NumPy operations rather than unnecessary Python-level loops.
- **Linear algebra:** Work with matrix operations, dot products, norms, and eigenvalue computations.
- **Memory awareness:** Understand views, copies, strides, and array contiguity.
- **Scientific computing:** Build a foundation for numerical methods, data analysis, and machine learning.
- **Problem-solving:** Develop the ability to choose appropriate NumPy operations for unfamiliar problems.

---

## ⚖️ Attribution & License

### Original Exercise Collection

The exercises are based on [100 NumPy Exercises](https://github.com/rougier/numpy-100), associated with Nicolas P. Rougier ([@rougier](https://github.com/rougier)) and contributions from the wider community.

Credit for the original exercises belongs to the respective authors and contributors.

### My Contributions

This repository contains my implementations, practice work, and any original explanations or comments included alongside the solutions.

### License

The license for this repository should be stated in accordance with the actual `LICENSE` file and the licensing terms applicable to the original materials.

If you intend to distribute the repository under the **BSD 3-Clause License**, include the appropriate license text and verify that the original materials and any reused content may be redistributed under those terms.

See [`LICENSE`](https://github.com/rougier/numpy-100/blob/master/LICENSE.txt) for the applicable license.

---

## 🙌 Final Note

One exercise at a time. One array at a time. One concept at a time.

The aim is not just to learn NumPy syntax, but to understand numerical computation well enough to apply it confidently in mathematics, data science, and machine learning.

**Happy coding! ⚡🐍**
