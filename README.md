# Simple Data Warehouse with Python, Pandas & SQLite

This project demonstrates how to build a **basic data warehouse** in Python using:

- **Pandas** for data manipulation  
- **SQLite3** for lightweight database storage  
- **Matplotlib & Seaborn** for data visualization  

It provides reusable functions to:
- Create and connect to an SQLite database
- Execute SQL queries and fetch results
- Convert Pandas DataFrames into database tables
- Perform simple data analysis (summary stats, missing values, etc.)
- Visualize data with bar, line, and scatter plots

---

## 🚀 Features
- **Database Connection**: Easily connect to SQLite databases  
- **Query Execution**: Run SQL queries with automatic commit  
- **Data Fetching**: Retrieve rows from SQL queries  
- **DataFrame Integration**: Store Pandas DataFrames as SQL tables  
- **Basic Analysis**: Quick overview of the dataset (head, info, stats, nulls)  
- **Visualization**: Plot bar, line, or scatter graphs with Seaborn  

---

## 📂 Project Structure
├── main.py # Main script (contains all functions and demo)
├── data_warehouse.db # SQLite database (auto-created when script runs)
└── README.md # Project documentation

---

🛠️ Future Improvements

Add support for CSV/Excel data import

Implement more advanced analytics (aggregations, groupby)

Expand visualization types (histograms, heatmaps, etc.)

Integrate with larger-scale databases (PostgreSQL, MySQL)

---

📜 License

This project is open-source and available under the MIT License.
