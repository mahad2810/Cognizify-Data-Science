# Data Science Internship: Restaurant Dataset Analysis and Predictive Modeling

## Overview
This project involves analyzing and modeling data from a restaurant dataset to gain insights and build predictive models. The tasks performed are structured across three levels: data exploration and preprocessing, descriptive and geospatial analysis, and predictive modeling with visualization. The primary objective is to analyze restaurant data, explore features, and build a regression model to predict the aggregate rating of restaurants.

---

## Level 1: Data Exploration and Preprocessing

### Objectives
1. Explore the dataset to identify rows and columns.
2. Handle missing values and invalid characters.
3. Convert data types as needed.
4. Analyze the target variable (“Aggregate rating”) and address any class imbalances.

### Key Steps
- Loaded the dataset using pandas.
- Removed rows containing non-ASCII characters in the `City` and `Address` columns.
- Calculated percentages of restaurants offering table booking and online delivery.
- Analyzed average ratings based on table booking availability and price range.
- Encoded categorical columns like `Has Table booking` and `Has Online delivery` for further analysis.

### Outputs
- Cleaned dataset saved as `modified_restaurants.csv`.

---

## Level 2: Descriptive and Geospatial Analysis

### Descriptive Analysis
- Calculated basic statistical measures (mean, median, standard deviation) for numerical columns.
- Explored distributions of categorical variables such as `Country Code`, `City`, and `Cuisines`.
- Identified top cuisines and cities with the highest number of restaurants.

### Geospatial Analysis
- Visualized restaurant locations using latitude and longitude.
- Analyzed restaurant distribution across cities and countries.
- Explored the correlation between location and ratings.

### Tools and Techniques
- Libraries: pandas, numpy, matplotlib, seaborn.
- Statistical measures and visualization techniques were used to understand trends and distributions.

---

## Level 3: Predictive Modeling and Data Visualization

### Predictive Modeling
- **Objective:** Build regression models to predict the aggregate rating of restaurants.
- **Features Used:**
  - Average Cost for Two
  - Price Range
  - Votes
  - Encoded `Has Table Booking`
  - Encoded `Has Online Delivery`

- **Models Implemented:**
  - Linear Regression
  - Decision Tree Regressor
  - Random Forest Regressor

- **Performance Metrics:**
  - Root Mean Squared Error (RMSE)
  - R-squared (R²)

| Model              | RMSE   | R²    |
|--------------------|--------|--------|
| Linear Regression  | Value  | Value  |
| Decision Tree      | Value  | Value  |
| Random Forest      | Value  | Value  |

### Data Visualization
- Histogram of `Aggregate Rating` distribution.
- Bar plot of top 10 cuisines by average rating.
- Comparative visualizations for ratings across cities and cuisines.

---

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn
- **Dataset Format:** CSV

---

## How to Run
1. Clone the repository and navigate to the project directory:
   ```bash
   git clone <repository_url>
   cd <repository_folder_name>
   ```
2. Install the required Python libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
3. Place the dataset (`Dataset.csv`) in the repository folder.
4. Open Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
5. Open the notebook file (`Level1.ipynb & Level3.ipynb`) and run the cells sequentially.

---

## Results and Insights
1. **Data Distribution:**
   - Most restaurants are concentrated in a few cities.
   - Online delivery is more prevalent in higher price ranges.

2. **Predictive Modeling:**
   - Random Forest performed best among the models tested.

3. **Visualization Insights:**
   - Specific cuisines and cities dominate high aggregate ratings.
   - Restaurant price range and features like table booking and online delivery influence ratings.

---

