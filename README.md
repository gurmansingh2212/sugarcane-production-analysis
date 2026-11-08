Sugarcane Production Analysis
A Python-based exploratory data analysis (EDA) project that studies sugarcane production across countries and continents. The notebook cleans the dataset, explores production-related indicators, and uses visualizations to compare production, cultivated area, and yield.
Project Overview
This project analyses a country-wise sugarcane production dataset to explore:
- Sugarcane production in tons
- Sugarcane production per person in kilograms
- Land area used for sugarcane cultivation (hectares)
- Sugarcane yield (kg per hectare)
- Distribution of countries across continents
- Differences in production and cultivated area between continents
- Relationships between numerical variables
Tools and Libraries
- Python – programming language
- Jupyter Notebook – interactive environment for analysis
- Pandas – data loading, cleaning, grouping, and analysis
- Matplotlib – plotting and visualization
- Seaborn – statistical charts and visualizations
Repository Contents
sugarcane-production-analysis/
├── Sugarcane_production.ipynb
├── List of Countries by Sugarcane Production.csv
├── README.md
└── requirements.txt
The CSV file is the dataset read by the notebook. Keep its filename unchanged unless you also update the pd.read_csv() path in the notebook.
Analysis Performed
1. Data Cleaning and Preparation
- Loads the CSV dataset using Pandas.
- Renames columns to make them easier to work with in Python.
- Removes formatting separators from numeric values and converts the relevant columns to numeric data types.
- Checks missing values, data types, and the number of unique values.
2. Univariate Analysis
- Counts the number of countries represented in each continent.
- Visualizes the continent-wise country count.
- Examines distributions of production, production per person, acreage, and yield.
- Uses box plots to inspect potential outliers.
- Generates descriptive statistics.
3. Country-Level Analysis
- Calculates each country's percentage contribution to total recorded production.
- Compares the top countries by production.
- Compares countries by cultivated acreage.
- Compares countries by yield per hectare.
- Examines production per person.
4. Correlation and Relationship Analysis
- Calculates correlations between numerical variables.
- Displays a correlation heatmap.
- Uses a scatter plot to examine the relationship between cultivated acreage and production.
5. Continent-Level Analysis
- Groups the data by continent.
- Compares total production and acreage across continents.
- Counts the number of countries represented in each continent.
- Explores the relationship between the number of countries and total production.
- Calculates correlations for the grouped continent-level data.
- Visualizes the distribution of production by continent.
Dataset
The notebook expects a CSV file named:

List of Countries by Sugarcane Production.csv

The dataset should include the columns used in the notebook:
- Country
- Continent
- Production (Tons)
- Production per Person (Kg)
- Acreage (Hectare)
- Yield (Kg / Hectare)
The notebook renames some columns during cleaning. If you obtain the dataset from another source or use a differently named file, update the file path and check that the column names match.
How to Run
1. Clone or download this repository.
2. Make sure Python is installed.
3. Install the required libraries:
   pip install -r requirements.txt
4. Open the project folder in Jupyter Notebook:
   jupyter notebook
5. Open Sugarcane_production.ipynb.
6. Run the notebook cells from top to bottom.
Requirements
The required Python packages are listed in requirements.txt:
- pandas
- seaborn
- matplotlib
- jupyter
Notes
- This is an exploratory data analysis project; it does not train or evaluate a machine learning prediction model.
- The charts and results depend on the dataset included in the repository.
- The notebook uses the Production per Person (Kg) column for one of its country-level comparisons. This is a per-person measure, not total sugarcane production.
- Make sure you have permission to redistribute the dataset before uploading the CSV to a public GitHub repository. If redistribution is not permitted, provide the dataset source and instructions for obtaining it instead.
Author
Gurman Singh
B.Tech Computer Science and Engineering (AI & ML) Student
