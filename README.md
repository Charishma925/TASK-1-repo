# Life Expectancy Data Cleaning and Preprocessing

This project demonstrates a step-by-step data cleaning and preprocessing pipeline using the **Life Expectancy** dataset from Kaggle. The goal is to prepare the raw data for machine learning tasks by handling missing values, encoding categorical variables, normalizing numerical features, and removing outliers.

## Dataset

- **Source**: Kaggle - Life Expectancy (WHO)
- **File**: `Life Expectancy Data.csv`

## Tools Used

- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-learn

## Preprocessing Steps

### 1. Import the Dataset and Explore Basic Info
- Load the CSV into a Pandas DataFrame.
- Use `.info()`, `.head()`, and `.isnull().sum()` to inspect structure and missing data.

### 2. Handle Missing Values
- Numerical columns: Filled using the **median** to reduce outlier impact.
- Categorical columns: Filled using the **mode** (most frequent category).

#### 3. Encode Categorical Features
One-hot encoding using pd.get_dummies() with drop_first=True to avoid multicollinearity.

##### 4. Normalize/Standardize Numerical Features
Standardization using StandardScaler() from sklearn.preprocessing to bring features to a mean of 0 and standard deviation of 1.

##### 5. Visualize and Remove Outliers
- Boxplots were used to detect outliers.
- Outliers removed using the Interquartile Range (IQR) method.

#### 6.Final Output
- A cleaned and preprocessed dataset ready for machine learning model training.
- Shape of the final dataset and data quality significantly improved.
