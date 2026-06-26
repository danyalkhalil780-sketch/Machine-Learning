Lab 2.1: Introduction to NumPy

Overview
This lab provides a comprehensive introduction to NumPy (Numerical Python), the fundamental package for scientific computing in Python. NumPy enables efficient numerical computations through its powerful N-dimensional array object and extensive mathematical functions.

Key Learning Objectives
Understanding NumPy arrays and their advantages over Python lists
Creating arrays using various methods (from lists, ranges, zeros, ones, etc.)
Performing array indexing, slicing, and selection operations
Implementing vectorized computations for efficient processing
Computing basic statistics and mathematical operations
Reshaping and manipulating arrays.

Key Topics
Topic	Functions/Methods
Array creation	np.array(), np.arange(), np.zeros(), np.ones(), np.linspace(), np.random.rand(), np.random.randint(), np.eye()
Indexing & slicing	arr[index], arr[start:stop:step], 2D [rows, cols]
Boolean masking	arr[arr > threshold], arr[(cond1) & (cond2)]
Vectorized ops	arr + scalar, arr * arr, np.sqrt(), np.log(), np.sin()
Statistics	.mean(), .std(), .var(), .sum(), .max(), .min(), .argmax(), .argmin(), np.median(), .cumsum()
Reshaping	.reshape(), .shape

Practice Exercises
Create an array of 10 zeros, 10 ones, 10 fives.
Generate integers from 10 to 50, then even numbers only.
Build a 3×3 matrix with values 0‑8 and a 3×3 identity.
Create a 10×10 matrix with values 0.01 to 1.00.
Generate 20 linearly spaced points between 0 and 1.
On a 5×5 matrix (1‑25), extract rows 2‑end and columns 1‑end.

Lab 2.2: Introduction to Pandas

Overview
This lab introduces Pandas, a powerful Python library for data manipulation and analysis. Pandas provides easy-to-use data structures and data analysis tools, making it essential for data science workflows, especially when dealing with structured data like CSV files.

Key Learning Objectives
Understanding Pandas DataFrame and Series structures
Creating DataFrames from dictionaries and external files
Basic data exploration and manipulation
Reading and writing CSV files
Data filtering and selection
Handling missing data and data cleaning
Grouping and aggregating data

Key Topics
Topic	Functions/Methods
DataFrame creation	pd.DataFrame(dict)
File I/O	df.to_csv(), pd.read_csv()
Exploration	.head(), .tail(), .describe(), .info(), .dtypes
Selection	df['col'], df[['col1','col2']], df.loc[row_label], df.iloc[row_pos], Boolean filtering
Manipulation	.rename(), .drop(), .reset_index()
Grouping	.groupby(), aggregate functions: .mean(), .sum(), .count(), .min(), .max()

Practice Exercises
Create a DataFrame with student data and save as CSV.
Read it back and display first 3 rows, last 2 rows.
Rename a column and drop an unnecessary column.
Filter rows where marks > 80.
Group by class and compute average marks and count.

Lab 2.3: Introduction to Matplotlib

Overview
This lab introduces Matplotlib, the most popular Python library for creating static, animated, and interactive visualizations. It provides a MATLAB-like interface for creating publication-quality charts and is highly customizable.

Key Learning Objectives
Creating basic and advanced plots with Matplotlib
Customizing plots with labels, titles, legends, and colors
Creating multiple plot types (line, bar, scatter, histogram, pie)
Using subplots to combine multiple visualizations
Adding aesthetic elements to make charts professional

Key Techniques
Topic	Methods
Date Extraction	.dt.normalize() to extract date from datetime
Data Merging	pd.merge() on 'Date' column
Holiday Dataset	Processed holiday CSV with 279 entries
Binary Feature Creation	.notnull().astype("int")
Feature Engineering	Add holiday indicator as 0 (normal) or 1 (holiday)

Holiday Dataset
Source: Processed US Federal holidays (2004–2018)
Total holidays: 279
Holidays in dataset range (Oct 2004 – Aug 2018): 258 holidays
Total holiday hours: 6,192 hours
