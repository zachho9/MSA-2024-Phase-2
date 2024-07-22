#### **1 Understand Dataset**
- Chose the W Store dataset, which was made of three sub-datasets.
- Extracted column names, data types, and non-null count from each sub-dataset.
- Converted datatype: "Date" to datetime, categorical cols ("IsHoliday" and "Type") to int.
- Plot each sub-dataset:
    - sales.csv:
        - Plotted box plots for weekly sales for 45 stores, showing the distribution.
        - Plotted weekly sales for selected store and department by defining a function.
    -  features.csv: Plotted 9 numerical data using sub-plots.
    -  stores.csv: Plotted store sizes data clearly showing 3 different types.

#### **2 Visualize Dataset, Identify Patterns and Anomalies**
- Explored more methods for visualization of each sub-datasets:
    - sales.csv:
        - Plotted weekly sales of all stores, comparing if IsHoliday.
        - Plotted monthly sales of all stores.
        - Plotted yearly sales of all stores.
    - features.csv: Plotted mean values of 9 features weekly, comparing if IsHoliday.
    - stores.csv: Plotted box plot of store sizes depending on the three types, showing the distribution.
- Patterns, anomalies:
    - Sales peaks at March-April, June-July, and December.
    - December had the best sales records in every year in the dataset.
    - Sales bottoms at January, May, and September-October.
    - Holiday sales often reached peak at the end of the year, often much better than nearby weeks. While holidays in other months did not have such pattern.
    - Data of MarkDown1-5 in features.csv showed clear outliers twice a year. These 5 columns also contained missing values.
    - The rest 4 numeric features in features.csv shows clear patterns. Temperature and Fuel Price show volatility during a year. While CPI and Unemployment showed linear trend.

#### **3 Data Cleaning and Identify Correlated Variables**
- Joined 3 sub-datasets into one dataframe.
- Dealed with missing values by removing MarkDown1-5 features.
- Dealed with outliers by identifying and removing the rows with outliers.
- Identified imbalanced data, which is type 2 (Type C) stores, but decided to if and how to deal with later.
- Identified correlated variables by plotting correlation matrix. Then removed Fuel_Price and Type columns due to high-correlation with other variables. This step also helped deal with imbalanced data by ignoring the store types.

#### **4 Save Cleaned Data**
- Checked data integrity and reset index.
- Added one hot encoding columns of IsHoliday in case it was needed for further usage.
- Save to local file.