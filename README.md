# Car Performance Analysis – Statistical & Visual Exploration

A detailed exploratory data analysis (EDA) on 32 classic car models, examining performance metrics such as mileage, horsepower, cylinders, weight, acceleration, and transmission type. This dataset is widely used for statistical modeling and machine-learning studies.

---

## Dataset Overview

The dataset contains **32 car models** and **12 performance-related attributes**, including:

- model  
- mpg (Miles per gallon)  
- cyl (Number of cylinders)  
- disp (Displacement)  
- hp (Horsepower)  
- drat (Rear axle ratio)  
- wt (Weight)  
- qsec (Quarter-mile time)  
- vs (Engine type: V/Straight)  
- am (Transmission: Automatic/Manual)  
- gear (Number of gears)  
- carb (Number of carburetors)  

---

## Data Preparation

Steps performed:

- Loaded dataset using pandas  
- Verified data shape (**32 × 12**)  
- Confirmed **no missing values**  
- Inspected data types of each column  
- Displayed initial and final rows for structural understanding  
- Extracted numeric columns for correlation analysis  
- Prepared data for visual and statistical exploration  

---

## Analysis & Visualizations

### Cylinders Distribution
Count plot showing frequency of 4-, 6-, and 8-cylinder cars.

### Horsepower Distribution
High variation across models; plotted with countplot for frequency understanding.

### Gear Distribution
3-gear cars are most common, followed by 4 and 5 gears.

### Model Count Plot
Each car model appears exactly once, validating dataset uniqueness.

### Correlation Heatmap
Key relationships identified:

- **mpg** is strongly **negatively correlated** with **wt** and **hp**  
- **hp** is strongly **positively correlated** with **disp**  
- **wt** correlates with **qsec** (heavier cars take longer to accelerate)  
- **am (manual transmission)** often aligns with higher mpg and drat  

---

## Key Insights

- Heavier and more powerful cars have significantly lower fuel efficiency.  
- Manual transmission cars tend to achieve better mileage.  
- 8-cylinder models dominate but perform poorly in mpg.  
- Displacement and horsepower rise together—large engines produce more power.  
- High-performance cars (e.g., Ferrari Dino, Maserati Bora) sacrifice fuel economy for speed.  
- 4-cylinder cars provide the best balance of efficiency, weight, and horsepower.  

---

## Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

---

## How to Run the Project

### Clone the Repository
` ` `bashgit clone https://github.com/yourusername/CarsAnalysis.git
### Install Required Packages
bash

Copy code

pip install pandas numpy matplotlib seaborn

Open the Notebook

bash

Copy code

jupyter notebook CarsAnalysis.ipynb

## Future Improvements
- Add a regression model to predict mpg

- Cluster cars into performance groups

- Build an interactive dashboard (Streamlit / Plotly)

- Add outlier detection and advanced statistical modeling

- Compare classic cars with modern vehicle datasets

---

## Contributing
Pull requests are welcome.
Feel free to add new insights, visualizations, or modeling approaches.

---

## Support
If you found this project helpful, consider starring the repository to support more data analysis work.
