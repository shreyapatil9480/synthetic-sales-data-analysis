# Synthetic Sales Data Analysis

This repository contains a self-contained project designed to showcase data analysis, visualization, and modeling skills for roles such as **Business Analyst**, **Program Manager**, and **Data Analyst**. The project uses a synthetic dataset representing sales transactions across different regions, customer segments, and product categories. A Jupyter Notebook guides you through exploratory data analysis (EDA), visualization, and the development of predictive models.

## Dataset

The synthetic dataset is stored in `synthetic_sales_data.csv` and includes the following columns:

| Column | Description |
| --- | --- |
| `OrderID` | Unique identifier for each order (1–1000) |
| `OrderDate` | Date of the order (between 2023-01-01 and 2024-12-31) |
| `Region` | Geographic region: North, South, East, or West |
| `CustomerSegment` | Customer type: Consumer, Corporate, Home Office, or Small Business |
| `ProductCategory` | Category of product sold: Electronics, Furniture, Clothing, or Food |
| `UnitCost` | Cost to acquire a single unit (USD) |
| `UnitPrice` | Selling price per unit (USD) |
| `UnitsSold` | Number of units sold in the transaction |
| `MarketingSpend` | Marketing spend associated with the transaction (USD) |
| `Profit` | Calculated profit: `(UnitPrice - UnitCost) * UnitsSold - MarketingSpend` (USD) |

This dataset was generated programmatically and does not represent real company data, making it safe for public use.

## Notebook: `analysis.ipynb`

The Jupyter Notebook walks through:

1. **Loading the data** – Importing the CSV file and displaying sample rows.
2. **Summary statistics** – Using `pandas` to explore distributions and descriptive statistics.
3. **Exploratory visualizations** – Creating bar charts, histograms, and scatter plots to uncover patterns in profits, units sold, and marketing spend.
4. **Predictive modeling** – Building and evaluating a Linear Regression and Random Forest model to predict profits. The notebook uses scikit‑learn pipelines with one-hot encoding for categorical features.
5. **Conclusion** – Summarizing insights and model performance.

## Getting Started

To run this project locally:

1. **Clone the repository**:
   ```bash
   git clone <REPO-URL>
   cd <REPO-NAME>
   ```
2. **Create a virtual environment (optional but recommended)**:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scriptsctivate`
   ```
3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
4. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook analysis.ipynb
   ```
5. Follow the notebook instructions to explore the data and models. Feel free to modify the notebook for further analysis or different predictive tasks.

## Requirements

All required Python packages are listed in `requirements.txt`. Key dependencies include:

- pandas
- numpy
- matplotlib
- seaborn
- scikit‑learn
- jupyter

You can install them via:

```bash
pip install -r requirements.txt
```

## License

This project is released under the MIT License. Feel free to use, modify, and share it for educational and professional portfolio purposes.

## Author


This project was created by an aspiring Business Analyst/Program Manager/Data Analyst seeking to demonstrate analytical skills.
## Contributing

Contributions are welcome! If you have ideas for improving the dataset, analysis, or models, feel free to fork the repository, create a feature branch, and submit a pull request.
