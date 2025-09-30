# OLAP Demo (ROLAP, MOLAP, HOLAP)

This repository demonstrates the core concepts of **Online Analytical Processing (OLAP)** using Python. OLAP is a key technique in Business Intelligence (BI) that allows users to perform **multidimensional analysis** of data, making it easier to uncover insights from datasets.

The demo focuses on:

* **ROLAP (Relational OLAP)** – Analysis using relational databases and SQL queries.
* **MOLAP (Multidimensional OLAP)** – In-memory cube-style aggregation with pandas.
* **HOLAP (Hybrid OLAP)** – Combining ROLAP and MOLAP approaches.

Additionally, it demonstrates common OLAP operations such as **slice, dice, roll-up, and drill-down** with accompanying **visualizations** using Seaborn and Matplotlib.

---

## 🔑 Key Concepts Demonstrated

### 1. ROLAP (Relational OLAP)

* Uses SQL queries on a relational database (SQLite).
* Example: calculating **average salary per department** using `GROUP BY`.
* Visualized with a **bar chart** showing department-level averages.

### 2. MOLAP (Multidimensional OLAP)

* Uses in-memory **pivot tables** with pandas.
* Example: creating a **salary cube** with `Department × Age` dimensions.
* Visualized with a **heatmap** for quick pattern recognition.

### 3. HOLAP (Hybrid OLAP)

* Combines relational queries with in-memory aggregations.
* Example: SQL extracts employee and department details, then pandas computes departmental averages.
* Visualized with a **bar chart** similar to ROLAP but backed by hybrid computation.

### 4. OLAP Operations

* **Slice** – Selects data for one dimension (e.g., employees in IT).
* **Dice** – Selects data for multiple conditions (e.g., HR employees with salary > 60,000).
* **Roll-up** – Aggregates data to a higher level (e.g., total salary per department).
* **Drill-down** – Explores data at a more detailed level (e.g., employee-level salaries within departments).

---

## 📂 Project Structure

```
├── olap_demo.py      # Main Python script (all OLAP operations & visualizations)
├── olap_demo.db      # SQLite database (auto-created when running the script)
├── README.md         # Project documentation
```

---

## ⚙️ Requirements

Make sure you have Python 3.7+ installed.
Install the required libraries:

```

> Note: `sqlite3` comes bundled with Python, no extra installation required.

```

**What happens:**

   * A SQLite database (`olap_demo.db`) is created with sample data (`employees` and `departments`).
   * OLAP operations (ROLAP, MOLAP, HOLAP) are performed.
   * Results are printed in the console.
   * Visualizations (bar plots, heatmaps) appear in separate windows.

---

## 📊 Example Outputs

* **ROLAP Result (SQL aggregation):**
  Average salary per department.

  ```
  department   avg_salary
  HR           93333.33
  Engineering  77500.00
  Sales        60000.00
  ```

  *(Displayed as a bar chart)*

* **MOLAP Cube:**
  Pivot table showing average salary by department vs age group.
  *(Displayed as a heatmap with annotated values)*

* **HOLAP Result:**
  Average salary per department using hybrid approach.

* **Slice Example:**
  Employees in the IT department.

* **Dice Example:**
  HR employees with salary > 60,000.

* **Roll-up Example:**
  Total salary per department (shown in a bar chart).

* **Drill-down Example:**
  Salary by employee, broken down by department (bar chart with hue).

---

## 🎨 Visualizations

The script generates several plots to help illustrate OLAP concepts:

* **ROLAP:** Bar chart of average salary by department.
* **MOLAP:** Heatmap of salary cube (Department × Age).
* **HOLAP:** Bar chart of hybrid aggregation.
* **Roll-up:** Bar chart of total salaries per department.
* **Drill-down:** Employee-level salary bar chart with department grouping.

---

## 📘 Learning Goals

This project is designed to help learners:

* Understand the differences between **ROLAP, MOLAP, and HOLAP**.
* See how **SQL** and **pandas** complement each other in OLAP contexts.
* Practice **data visualization** for analytical results.
* Get hands-on with **slice, dice, roll-up, and drill-down operations**.

---

## 📝 License

This project is open-source under the [MIT License](LICENSE).

---

## 🙌 Acknowledgments

* OLAP theory adapted from standard **Business Intelligence** concepts.
* Implemented with lightweight tools for **educational and demo purposes**.
