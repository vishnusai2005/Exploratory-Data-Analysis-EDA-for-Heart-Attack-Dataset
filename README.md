# Exploratory-Data-Analysis-EDA-for-Heart-Attack-Dataset
- Loaded and inspected the Heart Attack dataset to understand feature distributions and data types.
- Performed data cleaning by identifying and dropping 22 duplicate rows.
- Imputed missing values using the median for continuous numerical variables (`chol`, `thalachh`) and the mode for categorical variables (`exng`).
- Extracted descriptive statistics, calculating the mean, standard deviation, and quartiles (Q1, Q2, Q3) along with the Interquartile Range (IQR) for key metrics (`age`, `trtbps`, `chol`, `thalachh`).
- Conducted grouped analysis and created visualizations to determine heart attack risks based on gender (`sex`), resting electrocardiographic results (`restecg`), and ST/HR Slope (`slp`).
Functions and Plots Used
Pandas Functions & Methods:

Data Loading & Inspection: pd.read_csv(), .head(), .info()

Data Cleaning: .duplicated(), .sum(), .drop_duplicates(), .isnull(), .dropna(), .fillna()

Statistical Operations: .median(), .mode(), .mean(), .std(), .quantile()

Data Manipulation: .groupby(), .reset_index(), .replace(), .rename(), .values, .index

Visualization Functions (Seaborn & Matplotlib):

Plots:

sns.barplot(): Used to visualize the heart attack risk by categorical features like gender and resting ECG results.

sns.lineplot(): Used to visualize the average heart attack risk grouped by the ST/HR slope (slp).

Figure Styling & Display:

plt.figure(figsize=..., dpi=...): Used to set the dimensions and high resolution of the visualizations.

plt.title(): Used to add descriptive titles to the graphs.

plt.show(): Used to render the figures.
