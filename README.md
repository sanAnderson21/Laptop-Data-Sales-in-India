# Laptop Sales in India Dataset

## Overview
This dataset contains information about laptop sales in India, including details such as product names, prices, units sold, states, and other relevant features. It is designed for analysis, visualization, and machine learning tasks related to sales trends, regional preferences, and pricing strategies.

---

## Dataset Details

### File Name
- `dell_laptop_sales_india.csv`

### Columns
| Column Name         | Description                                   | Data Type |
|---------------------|-----------------------------------------------|-----------|
| `Year`              | Year of the sale                              | Integer   |
| `Month`             | Month of the sale                             | Integer   |
| `Model`             | Name of the laptop model                      | String    |
| `Price (INR)`       | Price of the laptop in Indian Rupees (INR)    | Integer   |
| `Units Sold`        | Number of units sold                          | Integer   |
| `State`             | State where the sale occurred                 | String    |
| `GNP (INR Crore)`   | Gross National Product (GNP) of the state     | Float     |
| `GST (%)`           | Goods and Services Tax (GST) rate             | Float     |
| `Inflation Rate (%)`| Inflation rate for the year                   | Float     |
| `Discount (%)`      | Discount offered on the laptop                | Float     |

### Example Data
| Year | Month | Model          | Price (INR) | Units Sold | State       | GNP (INR Crore) | GST (%) | Inflation Rate (%) | Discount (%) |
|------|-------|----------------|-------------|------------|-------------|-----------------|---------|--------------------|--------------|
| 2023 | 10    | Dell XPS 13    | 90000       | 150        | Maharashtra | 1200.5          | 18      | 5.5                | 10           |
| 2023 | 10    | Dell Inspiron  | 50000       | 200        | Karnataka   | 950.3           | 18      | 5.5                | 5            |

---

## Purpose
This dataset can be used for:
- Analyzing sales trends across different states in India.
- Understanding the impact of pricing, discounts, and inflation on sales.
- Building predictive models for sales forecasting.
- Visualizing regional preferences for laptop models.

---

## How to Use
1. **Download the Dataset**:
   - Click the `dell_laptop_sales_india.csv` file in the repository.
   - Click the "Download" button to save the file to your local machine.

2. **Load the Dataset**:
   - Use Python's `pandas` library to load the dataset:
     ```python
     import pandas as pd
     df = pd.read_csv('dell_laptop_sales_india.csv')
     print(df.head())
     ```

3. **Explore the Data**:
   - Perform exploratory data analysis (EDA) to understand the dataset's structure and trends.
   - Use visualization libraries like `matplotlib` or `seaborn` to create charts and graphs.

4. **Analyze or Model**:
   - Use the dataset for statistical analysis or machine learning tasks.

---

## Dataset Creation
This dataset was synthetically generated for educational and analytical purposes. It includes realistic features such as prices, units sold, and regional data to simulate real-world sales scenarios.

---

## License
This dataset is shared under the [MIT License](LICENSE). You are free to use, modify, and distribute the dataset for any purpose, but attribution is appreciated.

---

## Contributing
If you find any issues with the dataset or have suggestions for improvement, please open an issue or submit a pull request. Contributions are welcome!

---

## Acknowledgments
- This dataset was created for educational purposes.
- Inspired by real-world sales data and trends in the Indian market.

---

## Contact
For questions or feedback, please contact [Your Name] at [your.email@example.com].

---

## Example Code
Here’s an example of how to load and explore the dataset using Python:

```python
import pandas as pd
import matplotlib.pyplot as plt

# Load the dataset
df = pd.read_csv('dell_laptop_sales_india.csv')

# Display the first 5 rows
print(df.head())

# Plot sales by state
df.groupby('State')['Units Sold'].sum().plot(kind='bar', figsize=(10, 6))
plt.title('Total Units Sold by State')
plt.xlabel('State')
plt.ylabel('Units Sold')
plt.show()
