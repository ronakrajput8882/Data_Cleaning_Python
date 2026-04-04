<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=2,12,24&height=200&section=header&text=🧹%20Data%20Cleaning%20Python&fontSize=46&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Data%20Cleaning%20From%20Scratch%20|%20No%20Libraries%20|%20Pure%20Python&descAlignY=60&descAlign=50" width="100%"/>

<div align="center">

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)
[![No Libraries](https://img.shields.io/badge/Libraries-Zero-22c55e?style=for-the-badge&logo=python&logoColor=white)](#)
[![License](https://img.shields.io/badge/License-MIT-22c55e?style=for-the-badge)](LICENSE)

</div>

---

## 📌 Project Overview

**Data_Cleaning_Python** is a hands-on practice project that implements common data cleaning operations using **pure Python only — zero external libraries**. No Pandas, no NumPy, no shortcuts.

The goal is to deeply understand what happens under the hood when you clean real-world messy data — by building every step manually with core Python constructs like file I/O, string methods, list comprehensions, and custom logic.

> 💡 If you want to truly understand data cleaning, implement it without libraries first. That's exactly what this project does.

---

## 🔄 Pipeline Workflow

```
RAW_DATA.txt → Read & Parse → Clean & Transform → Validate → Write → CLEAN_DATA.txt
```

### 1️⃣ Load Raw Data
- Read `RAW_DATA.txt` using Python's built-in `open()` and `readlines()`
- Parse each line manually — no CSV readers, no DataFrames

### 2️⃣ Inspect & Identify Issues
- Detect missing/empty values by checking empty strings or placeholder tokens
- Identify inconsistent formatting (extra whitespace, mixed cases, special characters)
- Find duplicate rows using pure Python comparison logic

### 3️⃣ Clean & Transform
- **Strip whitespace** — `.strip()`, `.lstrip()`, `.rstrip()` on each field
- **Normalize casing** — `.lower()` / `.upper()` / `.title()` for consistency
- **Handle missing values** — replace blanks with defaults or remove rows
- **Remove duplicates** — track seen rows using a set-based approach
- **Fix data types** — validate and cast strings to int/float using `try/except`
- **Remove special characters** — manual character filtering with loops

### 4️⃣ Validate & Export
- Check cleaned records against expected format before writing
- Write cleaned output to `CLEAN_DATA.txt` using `write()` / `writelines()`

---

## 🔍 Key Insights

- 📌 **No-library constraint** forces deep understanding of how tools like Pandas `.dropna()`, `.drop_duplicates()`, and `.str.strip()` actually work internally
- 🔁 **Set-based deduplication** is O(1) lookup — much faster than nested loop comparison for large datasets
- ⚠️ **Type casting with `try/except`** is the cleanest pure-Python way to validate numeric fields without crashing on bad data
- 🧠 **String methods are powerful** — `.strip()`, `.split()`, `.replace()`, and `.join()` can handle 80% of text cleaning tasks with no imports at all

---

## 🗂️ Repository Structure

```
Data_Cleaning_Python/
│
├── DATA_CLENING_PRACTICE.ipynb   # Main Jupyter Notebook with all cleaning steps
├── RAW_DATA.txt                  # Input: messy, uncleaned raw dataset
├── CLEAN_DATA.txt                # Output: cleaned and validated dataset
└── README.md
```

---

## 🚀 Quick Start

```bash
# Clone the repo
git clone https://github.com/ronakrajput8882/Data_Cleaning_Python.git
cd Data_Cleaning_Python

# Launch the notebook (no installs needed — pure Python)
jupyter notebook DATA_CLENING_PRACTICE.ipynb
```

> ✅ No `pip install` required. Only Python 3.x and Jupyter Notebook.

---

## 🧠 Key Learnings

- Writing data cleaning logic from scratch builds intuition that makes Pandas and NumPy much easier to understand and debug
- Python's built-in string methods are surprisingly powerful for text normalization tasks
- Reading and writing structured text files manually teaches proper file handling, encoding awareness, and row-level control
- Using `set()` for deduplication and `try/except` for type validation are production-grade patterns even without libraries

---

## 🛠️ Tech Stack

| Tool | Purpose |
|:---|:---|
| Python 3.x | Core language — all logic built with standard library only |
| Jupyter Notebook | Interactive step-by-step execution and documentation |
| Built-in `open()` | File I/O for reading RAW_DATA and writing CLEAN_DATA |
| String methods | `.strip()`, `.lower()`, `.replace()`, `.split()` for text cleaning |
| `set` / `list` | Deduplication and row-level data management |
| `try/except` | Safe type casting and validation |

---

<div align="center">

### Connect with me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/ronaksinh-rajput8882)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/techwithronak)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ronakrajput8882)

*If you found this useful, please ⭐ the repo!*

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=2,12,24&height=100&section=footer" width="100%"/>

</div>