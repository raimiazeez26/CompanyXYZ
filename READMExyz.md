

# ANALYSIS OF SUPERMARKET DATA FOR COMPANY XYZ (ABUJA, LAGOS & PORTHARCOURT

Company XYZ owns a supermarket chain across the country. Each major branch located in 3 cities across the country recorded sales information for 3 months, to help the company understand sales trends and determine its growth, as the rise of supermarkets competition is seen.


# Project Steps

### 1. Loading Datasets
This step includes:
    - Importing Libraries (glob, os, pandas)
    - Using the "glob" library to match csv patterns
    - Combining all three datasets from the company using "pd.concat"  
    - Reading the csv file using "pd.read_csv"

### 2. Data Exploration
This step includes:
    - Import needed Libraries (Numpy, Seaborn, Matplolib)
    - Previewing the data usin ".head()"
    - Acessing the dataset to determine it's shape ("shape()") and number of columns (df.columns)
    - Getting the statistical summary of the dataset using ".describe()"
    - Checking for missing values using "isnull()"
    - Using "info()" to further explore the data observing the data types of each column and null values

### 3. DateTime Features
From the explorationsteps we observe the Date & Time columns are object data types and converted them to DateTime data type using "to_datetime"


### 4. Extracting Features from DateTime
- From the Date column, I extracted and appended the Day, Month and Year of each entry using the .dt.day, .dt.month & .dt.year fuctions respectively
- From the Time column, I extracted and appended the Hour of each entry using .dt.hour function
- I used "unique()" to check for unique value in the Hour column.

### 5. Unique Values 
- This step includes checking the unique values in each column using "unique()". This is to give further insight on the type and of variables in each column

### 6. Value Count
- This step includes counting the number of unique values using "counts.value()"

### 7. Aggregation by Groupby
- This step includes aggregation of our dataset by grouping then by City and sorting by gross income.



# Insights

Insights uncovered from visualization of the dataset includes: 

- Sales Record - Port Harcourt has the highesth sales record, follwed by Lagos and then Abuja.

- Payment Method - The most used payment method is Epay, followed closely by cash and then Card.

- Product Line - Fashon accessories are the highest selling product line followed by Food & Beverages.

- Produt Line by Payment Method - This shows that people who by Electronic accessories pay more by cash than any other group. People who buy Fahion, Home & Lifestyle & Health & Beauty Accessories pay more using Epay. Those who buy Food & Beverages pay more using card method

- Product Line by Branch - This Shows that the Lagos branch sold more Home & Lifestyle products compared to any other branch. Abuja branch sold more sport & Travel products compared to other branches and Port Hacourt branch sold more Food & Beverages compared to ther branches.

- Branch Rating  - This shows Lagos and Abuja branch have an qual rating above 7 and Abuja branch have a lower rating below 7.

- Product Line by Total sold based on Gender - This shows thast the stores have a higher number of female customers for all product line except Health & Beauty

- Quantity Sold Vs Unit Price - This shows no solid direct relationship between the quantity of items sold based on their unit price as product with a low unit price have low quantity sold. This implies that the quantity of items sold depends on other factors such as need rather than the unit price




# Future Work

- First task would be to find the error point between the Tax, Cost of Goods Sold & Gross Income and make correction to get right data for proper analysis on how to maximize gross income.

- I would like to collect data on major indivual products within each product line to find a corrolation between products that are bought together. This would guide in stocking the right quantity of products and help in creating discount packages and other loyalty packages.


# Standout Section

- Total sold by Hour of Day -  This shows that on the average more goods are sold between 18:00 & 20:00 hour of the day followed by between 12:00 & 14:00 hour.

- Total Sales by Month - This shows that more goods were sold in the 1st and 3rd Month compared respectively.

- Gross income by Product Line - This shows that the highest gross income were brought in by Home & Lifestyle and Sports & Travel product line respectively.

- Gross Income by Customer Type - As a measure of loyalty, customers who have membership card in the stores bring in more gross income than regular customers

Quantity sold per product line by customer type - This shows that members buy more food & beverages and health & beauty products compared to other products and regular customers buy more sports & Travel products.

Gross Income per month by Product Line - This shows that the stores sold more Food & Beverages, Electronics and Home & Lifestyle products in the first month. the stores sold and all time high record of sports & travel products.


# Executive Summary.

Included in the repository