
# Exploratory Data Analysis on World Population Data

In this project, I explored a world population dataset using Python libraries like Pandas, Seaborn, and Matplotlib. I wanted to get a better understanding of the data and its trends across different continents and over the years.

## What I Did

1. **Loaded and Cleaned the Data**  
   - Read the CSV file containing world population data.
   - Removed duplicate rows to ensure data quality.
   - Set up display options for better readability.

2. **Examined the Data**  
   - Checked basic information with `info()` and `describe()`.
   - Looked for missing values and counted unique entries.
   - Sorted the data to see the top 10 countries by "World Population Percentage".

3. **Analyzed Relationships**  
   - Calculated correlations between numeric features.
   - Visualized the correlations with a heatmap.

4. **Grouped and Compared Data**  
   - Grouped the data by continent to see average population values.
   - Focused on population trends over different years and plotted these trends.
   - Created a boxplot to understand the distribution of the data.
   - Made a scatter plot to explore the relationship between a country's area and its 2022 population.

## How to Run the Project

1. **Install Dependencies**  
   Make sure you have the necessary libraries:
   ```bash
   pip install pandas seaborn matplotlib
   ```

2. **Update the File Path**  
   Adjust the path to the CSV file in the code:
   ```python
   df = pd.read_csv(r"C:\Users\Admin\Downloads\world_population.csv")
   ```

3. **Run the Code**  
   You can run the code in your preferred Python environment (e.g., Jupyter Notebook, VSCode, or the command line).


## Final Thoughts

I enjoyed working on this project because it allowed me to dive into real-world data and uncover interesting trends and relationships.
