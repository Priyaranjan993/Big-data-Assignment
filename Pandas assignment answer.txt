# PandasAssignment


Q1. How do you load a CSV file into a Pandas DataFrame?
Ans: pd.read_csv("Path of the file")

Q2. How do you check the data type of a column in a Pandas DataFrame?
Ans: To check the data type in pandas DataFrame we can use the "dtype"  attribute. ex : df.dtype

Q3. How do you select rows from a Pandas DataFrame based on a condition?
Ans: Selecting rows based on particular column value using '>', '=', '=', '<=', '!=' operator.

Q4. How do you rename columns in a Pandas DataFrame?
Ans: Using rename() function .Exampale df.rename("emp":"EMP",inplace=True)

Q5. How do you drop columns in a Pandas DataFrame?
Ans : The drop() method removes the specified row or column.
       By specifying the column axis (axis='columns'), the drop() method removes the specified column.
example : dataframe.drop(labels, axis, index, columns, level, inplace., errors)
Q6. How do you find the unique values in a column of a Pandas DataFrame?
Ans : using unique() function .df['Courses'].unique()
Q7. How do you find the number of missing values in each column of a Pandas DataFrame?
 Ans: df.isnull()
Q8. How do you fill missing values in a Pandas DataFrame with a specific value?
Ans : df.fillna()
Q9. How do you concatenate two Pandas DataFrames?
 Ans: df1+df2
Q10. How do you merge two Pandas DataFrames on a specific column?
Ans: result = pd.merge(left, right, how="left", on=["key1", "key2"])
Q11. How do you group data in a Pandas DataFrame by a specific column and apply an aggregation function?
data.groupby('column_name')['column_name'].sum()
Q12. How do you pivot a Pandas DataFrame?
Ans: DataFrame.pivot(self, index=None, columns=None, values=None)
Q13. How do you change the data type of a column in a Pandas DataFrame?
Ans : df = df.astype(str)
Q14. How do you sort a Pandas DataFrame by a specific column?
Ans : using sort_value() function. df.sort_value()
Q15. How do you create a copy of a Pandas DataFrame?
Ans: using copy() function. newdf = df.copy()
Q16. How do you filter rows of a Pandas DataFrame by multiple conditions?
Ans:  There is multiple way to filter 1.where 2.loc[]
Q17. How do you calculate the mean of a column in a Pandas DataFrame?
Ans: df['column_name'].mean()
Q18. How do you calculate the standard deviation of a column in a Pandas DataFrame?
Ans: df['column_name'].std()
Q19. How do you calculate the correlation between two columns in a Pandas DataFrame?
Ans : By using corr() function. 
Q20. How do you select specific columns in a DataFrame using their labels?
Ans : df[["column1","column2"]]
Q21. How do you select specific rows in a DataFrame using their indexes?
Ans : using the loc[] function
Q22. How do you sort a DataFrame by a specific column?
df.sort_value(by="column_name",ascendig=False)
Q23. How do you create a new column in a DataFrame based on the values of another column?
Ans:We can use DataFrame.apply()
Q24. How do you remove duplicates from a DataFrame?
Ans: dataframe.drop_duplicates(subset, keep, inplace, ignore_index)
Q25. What is the difference between .loc and .iloc in Pandas?
Ans: The main difference between pandas loc[] vs iloc[] is loc gets DataFrame rows & columns by labels/names and iloc[] gets by integer Index/position. For loc[], if the label is not present it gives a key error. For iloc[], if the position is not present it gives an index error.