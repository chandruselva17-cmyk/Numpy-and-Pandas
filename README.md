# Numpy-and-Pandas

Data Analysis with NumPy and Pandas

A hands-on assignment on numerical computing and structured data analysis in Python. It uses NumPy to analyze two weeks of daily temperature readings, and Pandas to work with a ranked marks Series and a retail transactions dataset.

Table of Contents

Objectives

Tasks Covered

Part 1: NumPy Array Operations

Part 2: Pandas Series

Part 3: Pandas DataFrame

Datasets

Key Concepts Practiced

Objectives

Work with NumPy arrays for numerical computations

Use Pandas Series and DataFrame for data manipulation and analysis

Apply indexing, slicing, filtering, and aggregation techniques

Understand real-world data handling through temperature and transaction datasets

Tasks Covered

Part 1: NumPy Array Operations

Scenario: Analyze daily average temperatures (°C) recorded over two weeks.

Create a 1D array temperatures_w1 for Week 1: [22.5, 25.3, 20.8, 23.4, 26.1, 24.8, 21.9]

Inspect properties: shape, data type, and number of elements

Array operations

Convert Celsius to Fahrenheit: F = (C * 9/5) + 32

Find the maximum, minimum, and mean temperature for the week

Slicing and indexing

First three days of the week

Weekend (last two days)

Middle three days of the week

Create a 2D array temperatures with one row per week

Week 1: [22.5, 25.3, 20.8, 23.4, 26.1, 24.8, 21.9]

Week 2: [19.2, 22.5, 21.3, 24.0, 23.5, 22.8, 20.1]

Inspect and slice the 2D array

Shape, data type, and total number of elements

Extract each week's temperatures and the weekend (last two days) of both weeks

Part 2: Pandas Series

Create a Series marks with values 95, 92, 89, 85, 80 and custom index Rank1 to Rank5

Indexing and slicing

Access the 1st rank student's mark by integer position
Use loc to get the marks of the top 3 ranks by label
Use iloc to get the 3rd-ranked student's mark
Apply a boolean mask to find ranks with marks greater than 90

Manipulating the Series

Change the 1st rank's mark to 100

Remove the entry for the last rank

Compute CGPA by dividing each mark by 10

Part 3: Pandas DataFrame

Create the DataFrame transactions (see Datasets)

Data exploration

Display the DataFrame with head, tail, shape, column names, and data types

Select only the ProductCategory and Amount columns

Retrieve the last 3 columns using iloc or loc

Filter rows where Region is 'North' and Amount > 200

Value counts for ProductCategory

Unique values in Region

Group by Region and compute the mean Amount

Manipulating the DataFrame

Update Amount to 165 for TransactionID 102

Add a Discount column equal to 10% of Amount

Remove the row with TransactionID 109

Delete the Discount column

Datasets

Temperatures (°C)

Week	Day 1	Day 2	Day 3	Day 4	Day 5	Day 6	Day 7
1	22.5	25.3	20.8	23.4	26.1	24.8	21.9
2	19.2	22.5	21.3	24.0	23.5	22.8	20.1

Transactions

TransactionID	ProductCategory	Region	Amount
101	Electronics	North	200
102	Clothing	South	150
103	Electronics	North	300
104	Furniture	East	450
105	Clothing	West	200
106	Electronics	North	250
107	Furniture	East	300
108	Clothing	West	180
109	Furniture	South	350
110	Electronics	North	400

Key Concepts Practiced

NumPy: np.array, .shape, .dtype, .size, vectorized arithmetic, max/min/mean, 1D and 2D slicing

Pandas Series: custom indices, positional vs. label-based access, loc, iloc, boolean masking, element-wise operations, drop

Pandas DataFrame: head/tail/info, column selection, iloc/loc, conditional filtering, value_counts, unique, groupby, adding/updating/removing rows and columns
