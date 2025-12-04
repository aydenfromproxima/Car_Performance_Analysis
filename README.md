# Car_Performance_Analysis

**Dataset Overview**

The dataset contains 32 car models with 12 performance-related attributes, widely used for statistical and machine learning studies.

Features include:

model

mpg (Miles per gallon)

cyl (Number of cylinders)

disp (Displacement)

hp (Horsepower)

drat (Rear axle ratio)

wt (Weight)

qsec (1/4 mile time)

vs (Engine type: V/Straight)

am (Transmission: Automatic/Manual)

gear (Number of gears)

carb (Number of carburetors)

Data Preparation

In the notebook, I:

 Loaded the dataset using pandas
 Checked data shape → 32 rows × 12 columns
 Verified no missing values
 Checked data types for all columns
 Displayed first and last few rows for structure understanding
 Extracted numeric columns for correlation analysis
 Prepared data for visual exploration

**Analysis & Visualizations**

The notebook includes multiple visualizations and statistical summaries:

1. Cylinders Distribution

Count plot showing distribution of 4-, 6-, and 8-cylinder vehicles.

2. Horsepower Distribution

High variation in horsepower across car models.
Count plot used for basic frequency overview.

3. Gear Distribution

3-gear cars are the most common, followed by 4 and 5 gears.

4. Model Count Plot

Shows each car model appears once (as expected), verifying dataset uniqueness.

5. Correlation Heatmap

A heatmap revealed key relationships:

mpg is strongly negatively correlated with wt and hp
hp is positively correlated with disp
wt is highly correlated with qsec (acceleration time)
am (manual) tends to be associated with higher mpg and drat

**Key Insights**

Cars with higher weight and horsepower have lower mileage (mpg).
Manual transmission (am = 1) often corresponds to better fuel efficiency.
Cars with 8 cylinders dominate the dataset but show poor fuel economy.
Displacement and horsepower move together—larger engines produce more power.
Performance cars (like Ferrari Dino, Maserati Bora) have high hp but lower mpg.
Cars with 4 cylinders demonstrate the best balance of mpg, weight, and hp.

Language & Libraries Used

Python
Pandas
NumPy
Matplotlib
Seaborn

**Jupyter Notebook**

**How to Run**
Clone the repository:
git clone https://github.com/yourusername/CarsAnalysis.git

Install required packages:
pip install pandas numpy matplotlib seaborn

Open the notebook:
jupyter notebook CarsAnalysis.ipynb

**Future Improvements**

Add regression model to predict mpg
Cluster cars into performance groups
Build an interactive dashboard (Streamlit / Plotly)
Add outlier detection & deeper statistical modeling
Compare classic cars with modern datasets

Contributing

Pull requests are welcome!
Feel free to add insights, new visualizations, or modeling approaches.

If You Found This Useful

Star the repository to support more data analysis projects!
