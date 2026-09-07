# Analyzing the Job Market: Trends, Skills, and Insights (10/2025 - 11/2025)

> **Course Assignment / Project:** Data Analysis Project  
> **Author:** Võ Hoàng Thịnh  
> **Institution:** Ho Chi Minh City Open University  
> **Major:** Computer Science (Data Science)  

---

## 1. Introduction
Amidst the highly competitive recruitment market for Data Analytics, accurately capturing technology trends, skill demands, and salary benchmarks is critical for a Data Analyst's career path.

This project collects, cleans, and mines data from thousands of real job postings to address key questions:
* Which programming languages and tools dominate the job market?
* How are average compensations and payment structures (hourly vs. annual) distributed?
* What core skills are absolute must-haves for an intern or entry-level Data Analyst?

---

## 2. Tech Stack
The project is implemented entirely in **Python** within a **Jupyter Notebook** environment, utilizing robust libraries for data processing and visualization:
* **Data Manipulation:** `Pandas`, `NumPy`
* **Natural Language Processing & Tokenization:** `NLTK` (`word_tokenize`, `MWETokenizer`) for extracting skill keywords from job descriptions.
* **Data Visualization:** `Matplotlib` for generating professional statistical charts.

---

## 3. Data Pipeline & Preprocessing
The raw dataset (`gsearch_jobs.csv`) underwent rigorous technical processing steps:
1. **Data Cleansing:** Filtered out null values, standardized date formats (`datetime`), and removed noise characters.
2. **Salary Standardization:** 
   * Split raw salary strings into minimum (`salary_min`), maximum (`salary_max`), average (`salary_avg`), and rate (`salary_rate`).
   * Converted hourly and monthly rates into a uniform standard metric: **Annualized Salary (`salary_standardized`)** for straightforward comparison.
3. **Keyword Tokenization:** Utilized `NLTK` to lowercase job descriptions, tokenize text, handle multi-word expressions (e.g., *Power BI*, *Data Lake*, *Machine Learning*), and filter against a standard keyword dictionary (Programming languages, Libraries, Analyst tools, Cloud tools).

---

## 4. Key Findings & Insights
### A. Dataset Overview
* **Total Records:** 1,820 job postings analyzed.
* **Collection Span:** Data monitored across an extended chronological timeframe to ensure market neutrality.

### B. Top Essential Programming Languages for Data Analysts
Frequency analysis of programming languages mentioned across job postings highlights the absolute dominance of core toolsets:

![Top Programming Languages](image_4e1c9c.png)

* **SQL (~55% of job postings):** Maintains its crown as the most crucial skill, required for querying and extracting data from relational databases.
* **Python (~32%):** The leading programming language for data cleansing, automation, and analytical modeling.
* **R (~24%):** Retains steady demand within research and advanced statistical environments.
* **SAS & Others:** Lower representation, typically catering to financial institutions or legacy corporate systems.

> **💡 Business Insight:** For students and applicants targeting **Data Analyst Intern** positions, mastering the **SQL & Python** duo is a prerequisite to passing resume screens at over half of the hiring companies.

---

## 5. How to Run
1. Clone this repository:
   ```bash
   git clone [https://github.com/Th1nhph0/analyzingJobMarket.git](https://github.com/Th1nhph0/analyzingJobMarket.git)

  Install dependencies:

```bash
pip install pandas numpy matplotlib nltk

Open the complete source code notebook to explore charts and analytical steps in detail:

Jupyter Notebook: PTDL.ipynb
