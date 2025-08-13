Hospital Dataset Visualization & Analysis

It is a "Python-based data visualization and statistical analysis project" that explores a hospital dataset.
I used pandas,seaborn, matplotli, and scipy to perform data cleaning, generate visualizations, and run statistical tests
to uncover insights about patient demographics, medical conditions, billing, and hospital stay patterns

 FEATURES
"Data Cleaning & Preprocessing"

  * Converts admission and discharge dates to 'datetime' format.
  * Calculates "length of stay" for each patient.
  * Handles categorical encoding for correlation analysis.

* "Data Exploration"

  * Displays basic dataset information, statistics, and missing values.

* "Visualizations"

  1. Blood Type Distribution – Bar chart of patient blood types.
  2. Medical Condition Frequency – Count plot of the most common conditions.
  3. Average Billing Over Time – Line chart showing yearly trends.
  4. Billing by Admission Type – Box plot comparison.
  5. Age Distribution by Gender – Histogram with FacetGrid.
  6. Correlation Matrix – Heatmap of numeric & encoded categorical variables.
  7. Pairplots – Scatter matrix of numerical features (with and without gender hue).
  8. Blood Type Pie Chart – Patient percentage distribution.

# Statistical Analysis

  * Performs a 'T-test' to compare billing amounts between male and female patients.

  "Technologies Used"

* "Python 3.x"
* Pandas – Data loading and preprocessing
* NumPy – Numerical operations
* Seaborn – Statistical visualizations
* Matplotlib – Plotting
* SciPy – Statistical tests

# Project Structure

hospital_analysis.py   # Main script with all visualizations and analysis
hospital.csv           # Dataset file

# Installation & Setup

1. Clone the repository

   bash
   git clone https://github.com/hemanthcharano/hospital-data-visualization.git
   cd hospital-data-visualization
   
2. Install dependencies

   bash
   pip install pandas numpy seaborn matplotlib scipy
   
3. Place your dataset

   * Save 'hospital.csv' in the same directory as the script.
   * Ensure it contains columns like:
     Date of Admission, Discharge Date, Blood Type, Medical Condition,
     Age, Billing Amount, Admission Type, Gender, Room Number
     
4. Run the script
   bash
   python hospital_analysis.py

# How It Works

1. Loads the CSV dataset into a pandas DataFrame.
2. Preprocesses dates and computes the stay length.
3. Generates multiple visualizations for different insights.
4. Performs a T-test to check if billing amounts differ significantly by gender.
5. Displays results and plots sequentially.
   
#  Example Output

* "Blood Type Distribution"
  A pastel bar chart showing the count of patients per blood type.
* "Average Billing Over Years"
  A line chart highlighting billing trends over time.
* "T-test Result"

  T-test result: t = -1.45, p = 0.1482

  Interpretation: No statistically significant difference in billing between genders (at 5% significance level).

 *Notes

* The dataset file 'hospital.csv' is **not included** in this repository for privacy reasons.
* Ensure date columns in the dataset are in a format recognizable by 'pandas.to_datetime()'.
* Some visualizations may require enough data diversity (e.g., at least two genders or multiple years).
