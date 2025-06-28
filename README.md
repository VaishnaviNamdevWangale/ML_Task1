📑 Table of Contents
* Introduction to Pandas
* Creating DataFrames
* Viewing Data
* Accessing Rows and Columns
* Filtering Data
* Sorting Data
* Adding and Removing Columns
* Basic Statistics
* Grouping Data
* Real-world Example (if applicable)


🧪 Step-by-step Description
1. Importing Pandas
import pandas as pd
The pandas library is imported with the alias pd.

2. Creating a DataFrame
data = {
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Age': [25, 30, 35],
    'City': ['New York', 'Los Angeles', 'Chicago']
}
df = pd.DataFrame(data)
A dictionary is created and passed to pd.DataFrame() to form a table-like structure.

3. Displaying the DataFrame
print(df)
This prints the entire DataFrame to the console/output.

4. Accessing Columns
print(df['Name'])
Displays only the Name column values.

5. Accessing Rows (loc / iloc)
print(df.loc[0])
print(df.iloc[1])

loc[] is used for label-based access.
iloc[] is used for position-based access.

6. Filtering Rows
print(df[df['Age'] > 28])
Shows only rows where Age is greater than 28.

7. Sorting Values
print(df.sort_values('Age'))
Sorts the DataFrame based on the Age column in ascending order.

8. Adding New Column
df['Salary'] = [50000, 60000, 70000]
Adds a new column Salary to the DataFrame.

9. Dropping Column
df = df.drop('City', axis=1)
Removes the City column using drop().

10. Summary Statistics
print(df.describe())
Displays basic statistics like mean, standard deviation, min, max, etc., for numeric columns.

11. Grouping Data (if available)
df.groupby('some_column').mean()
Groups the DataFrame by a column and calculates the mean of each group.

