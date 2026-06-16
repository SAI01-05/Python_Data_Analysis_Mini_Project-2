# IPL 2026 Analysis — First 39 Matches Using Python

<p align="center">
  <img src="images/Life_cycle.png" alt="Data Analytics Life Cycle" width="420"/>
</p>


---

## Project Overview

A beginner-level Exploratory Data Analysis (EDA) project built while learning Python for Data Analytics. The dataset contains records from the first 39 matches of IPL 2026 and is analyzed using core Python libraries.

The project is structured around the **Data Analytics Life Cycle**:

```
Objective → Understanding the Data → Data Cleaning & Transformation → Data Analysis → Data Visualization → Insights
```

---

## Objective

- Analyze team performances during the first 39 matches of IPL 2026
- Identify the teams with the highest number of wins
- Compare matches won while defending and chasing
- Discover players with the most Player of the Match awards
- Analyze top-scoring batters
- Examine the best bowling performances

---

## Dataset

| Field       | Details                         |
|-------------|---------------------------------|
| Source      | [kaggle](https://www.kaggle.com/) |
| File        | `1-39_Record_Dataset-IPL2026.csv`            |
| Records     | 39                              |
| Columns     | 23                              |
| Tournament     | IPL 2026                     |
| Matches Covered     | First 39 Matches        |

**Column Reference:**

| Column                | Description                      |
|-----------------------|----------------------------------|
| `Product Name`        | Full iPhone model name           |
| `Product URL`         | Flipkart listing link            |
| `Brand`               | Apple                            |
| `Sale Price`          | Current selling price (INR)      |
| `MRP`                 | Maximum Retail Price (INR)       |
| `Discount Percentage` | Discount offered (%)             |
| `Number Of Ratings`   | Total customer ratings           |
| `Number Of Reviews`   | Total written reviews            |
| `UPC`                 | Unique product code              |
| `Star Rating`         | Average star rating (out of 5)   |
| `RAM`                 | Device RAM                       |

---

## Libraries Used

```python
import pandas as pd               # Data loading, cleaning, exploration
import numpy as np                # Numerical operations
import plotly.express as px       # Interactive charts and visualizations
import plotly.graph_objects as go # Custom graph objects
```

---

## What I Learned

**Pandas**
- Loading CSV files using `pd.read_csv()`
- Exploring data with `data.head()`, `data.shape`, `data.info()`
- Checking for missing values using `data.isnull().sum()`
- Statistical summary using `data.describe()`
- Sorting records using `data.sort_values()`
- Selecting and filtering specific columns from a DataFrame

**NumPy**
- Numerical operations on DataFrame columns
- Understanding data types and basic statistical measures

**Plotly**
- Creating interactive bar charts using `plotly.express`
- Building scatter plots with OLS trendlines using `trendline="ols"`
- Using the `size` parameter for bubble-style scatter plots
- Customizing chart titles and axis labels

**EDA Concepts**
- Following the Data Analytics Life Cycle
- Exploring and understanding an unfamiliar dataset
- Deriving insights through sorting, filtering, and visualization

---

## Analysis and Visualizations

### 1. Numbers of Ratings — Highest Rated iPhones

Bar chart showing which top-rated iPhone models received the most customer ratings.

<p align="center">
  <img src="images/newplot.png" alt="Number of Ratings Bar Chart" width="760"/>
</p>

**Insight:** The iPhone 8 Plus (Gold, 64 GB) has the highest number of ratings among the top-rated models, indicating strong sales volume.

---

### 2. Numbers of Reviews — Highest Rated iPhones

Bar chart comparing the number of written reviews for top-rated iPhone models.

<p align="center">
  <img src="images/newplot_1_.png" alt="Number of Reviews Bar Chart" width="760"/>
</p>

**Insight:** The iPhone 8 Plus also leads in total reviews, reflecting high customer engagement on Flipkart.

---

### 3. Relationship Between Sale Price and Number of Ratings

Scatter plot with trendline examining how price affects the volume of customer ratings.

<p align="center">
  <img src="images/newplot_2_.png" alt="Sale Price vs Number of Ratings" width="760"/>
</p>

**Insight:** Lower-priced models such as the iPhone SE and iPhone 11 have significantly more ratings, suggesting higher purchase volumes at accessible price points.

---

### 4. Relationship Between Discount Percentage and Number of Ratings

Scatter plot with OLS trendline showing how discount levels relate to customer rating counts.

<p align="center">
  <img src="images/newplot_3_.png" alt="Discount Percentage vs Number of Ratings" width="760"/>
</p>

**Insight:** Products offering higher discounts tend to accumulate more ratings, indicating that discounts drive purchase volume and customer feedback.

---

## Project Structure

```
Python_Data_Analysis_Mini_Project/
|
|-- images/
|   |-- Life_cycle.jpeg                      # Data Analytics Life Cycle reference
|   |-- newplot.png                          # Bar chart — Ratings
|   |-- newplot_1_.png                       # Bar chart — Reviews
|   |-- newplot_2_.png                       # Scatter — Sale Price vs Ratings
|   |-- newplot_3_.png                       # Scatter — Discount % vs Ratings
|
|-- apple_products.csv                       # Dataset
|-- I-Phone_dataAnalysis_Using_Python.ipynb  # Main Jupyter Notebook
|-- README.md                                # Project documentation
```

---

---

## Author

**Sai Halwai**  
B.Sc. Computer Science — Game Design & Development  
Shree SaiBaba College, Shirdi

- Email: saihalwai01@gmail.com  
- GitHub: [SAI01-05](https://github.com/SAI01-05)  

---

*This is a learning project built while exploring Python for Data Analytics. More projects coming soon.*
