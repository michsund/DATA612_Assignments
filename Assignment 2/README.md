# Module 2 Assignment
For this assignment I again worked with the State Druge Utilization Data.  I started the assignment by importing the data set and necessary packages, then showing the top row of data to obtain a visual of column names and data representations.  

To retrieve the max date in the "Quarter Begin Date" column, I defined "qdate" to call on the column easier, then used the .max() function to obtain the latest date listed in the column.  In order to find the difference between the dates in the qdate column and the max date, I had to convert the dates to datetime type.  I used the pd.to_datetime function to achieve this, using the format '%m/%d/%Y' to match the existing format in the data.  I then performed the calculation of the difference between max date and all dates in the column, defining the calculation as "daydif".

In order to convert the difference in days, I used the numpy function np.timedelta64 to represent the time difference in months instead.  I defined this calculation as a new column in the data set "Max Date Difference", and displayed the first two rows to show the change.  Finally, I saved the data set as a CSV file using the to_csv function.
