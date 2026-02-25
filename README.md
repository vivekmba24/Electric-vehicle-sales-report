# India EV Sales Analysis

An exploratory data analysis of electric vehicle (EV) sales across Indian states from 2014 to 2024.

## Dataset

**File:** `Data.csv`

**Shape:** 96,845 rows × 8 columns

| Column | Type | Description |
|---|---|---|
| `Year` | float64 | Year of sale |
| `Month_Name` | str | Month of sale (e.g., `jan`) |
| `Date` | str | Full date of record |
| `State` | str | Indian state |
| `Vehicle_Class` | str | Specific vehicle class (e.g., BUS, AMBULANCE) |
| `Vehicle_Category` | str | Broad category (2-Wheelers, 3-Wheelers, etc.) |
| `Vehicle_Type` | str | Vehicle type grouping |
| `EV_Sales_Quantity` | float64 | Number of EVs sold |

## Key Findings

### Total Sales
- **3,593,811** EVs sold across all years and states.

### Year-over-Year Growth

| Year | Sales |
|---|---|
| 2014 | 2,392 |
| 2015 | 7,805 |
| 2016 | 49,855 |
| 2017 | 87,420 |
| 2018 | 130,254 |
| 2019 | 166,819 |
| 2020 | 124,684 *(COVID-19 dip)* |
| 2021 | 331,498 |
| 2022 | 1,024,723 |
| 2023 | 1,525,179 |
| 2024 | 143,182 *(partial year)* |

### Top 10 States by EV Sales

| State | Sales |
|---|---|
| Uttar Pradesh | 732,074 |
| Maharashtra | 401,535 |
| Karnataka | 315,498 |
| Delhi | 268,538 |
| Rajasthan | 228,573 |
| Bihar | 213,465 |
| Tamil Nadu | 206,902 |
| Gujarat | 176,713 |
| Assam | 151,917 |
| Kerala | 133,246 |

### Sales by Vehicle Category

| Category | Sales |
|---|---|
| 2-Wheelers | 1,808,105 |
| 3-Wheelers | 1,620,310 |
| 4-Wheelers | 149,775 |
| Others | 8,612 |
| Bus | 7,009 |

2-Wheelers and 3-Wheelers together account for **~95%** of all EV sales.

## Notebook Structure

1. **Data Loading** — Read CSV, preview with `df.head()`
2. **Exploration** — Shape, dtypes, column names via `df.info()`
3. **Cleaning** — Cast `Year` to `int`, parse `Date` to datetime, verify no nulls or duplicates
4. **Analysis**
   - Total EV sales
   - Sales by year
   - Top 10 states
   - Sales by vehicle category
5. **Visualisation** — Line and bar charts using `matplotlib`

## Requirements

```
pandas
matplotlib
```

## Usage

```bash
jupyter notebook Notebook.ipynb
```

> Ensure `Data.csv` is in the same directory as the notebook before running.
