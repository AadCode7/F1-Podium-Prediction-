
# Formula 1 Race Outcome Prediction

This project analyzes historical Formula 1 racing data to explore driver performance and build a machine learning model that predicts race finishing positions. It combines real-world motorsport data, exploratory data analysis (EDA), and predictive modeling techniques.

## Technologies Used

- **Python**: Core programming language for data processing and analysis.
- **Pandas & NumPy**: Used for structured data manipulation, merging datasets, handling missing values, and efficient numeric computations.
- **Matplotlib & Seaborn**: For data visualization — histograms, scatter plots, and heatmaps help interpret relationships and distributions.
- **Scikit-learn**: Used for:
  - Preprocessing: `LabelEncoder`, `StandardScaler`, `MinMaxScaler`
  - Model training: `RandomForestClassifier`
  - Model evaluation: `accuracy_score`, `confusion_matrix`, and `classification_report`
- **Jupyter Notebook**: For an interactive environment to explore, document, and visualize insights.

## What the Code Does

1. **Loads Raw Data**:
   - Merges multiple CSV files: `drivers.csv`, `results.csv`, `races.csv`, and `constructors.csv`.

2. **Data Exploration & Cleaning**:
   - Checks for missing values.
   - Encodes categorical features like driver names and constructor IDs.
   - Visualizes the distribution of grid and finishing positions using histograms.

3. **Driver Performance Focus**:
   - Filters and visualizes data for three specific drivers: **Fernando Alonso, Lewis Hamilton, and Kimi Raikkonen**.
   - Shows how often each driver starts from certain grid positions and how often they finish in specific positions.
   - Uses scatter plots to analyze the relationship between starting grid and final position.

4. **Feature Engineering**:
   - Creates new features like driver experience and race experience based on the year.
   - Helps the model learn trends related to experience over time.

5. **Machine Learning Model**:
   - Trains a `RandomForestClassifier` to predict a driver’s race finishing position based on:
     - Starting grid position
     - Constructor ID
     - Circuit ID
     - Driver ID
     - Year
     - Experience metrics
   - Evaluates model accuracy and visualizes confusion matrix.

6. **Feature Importance**:
   - Visualizes how much each feature contributes to prediction accuracy.

## Visualizations

- Grid vs. Finishing position scatter plot with inverted Y-axis (since P1 is the goal).
- Driver-specific histograms to understand qualifying vs. performance.
- Confusion matrix heatmap to evaluate model prediction capability.
- Bar chart showing feature importance.

## How to Run

1. Clone the repo
2. Place the data CSV files in the same directory
3. Open the notebook using Jupyter
4. Run all cells sequentially to explore the insights and generate predictions


