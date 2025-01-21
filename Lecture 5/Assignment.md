## Assignments

1. Basic Dataframe Operations
   - Create a data frame using a dictionary
     
        ```Python
        
        import pandas as pd
        dict = {
             'Month': ['Jan','Feb','Mar','Apr','May','June','July','Aug','Sept','Oct','Nov','Dec'],
             'Days': [31,28,31,30,31,30,31,31,30,31,30,31]
        }
        df = pd.DataFrame(dict)

        ```
        
        ![Output](https://github.com/mg270524/Data-Analytics-with-Python/blob/main/Lecture%205/assignment_outputs/Screenshot%20from%202025-01-21%2016-00-34.png)
   - Display the first five rows of the data frame
     ```Python
     
        df.head(5)
     
     ```
     ![Output](https://github.com/mg270524/Data-Analytics-with-Python/blob/main/Lecture%205/assignment_outputs/Screenshot%20from%202025-01-21%2016-07-32.png)
     
   - Retrieve the shape, column names, and data types of the data frame
     ```Python
     
        df.columns
     
     ```
     ![Output](https://github.com/mg270524/Data-Analytics-with-Python/blob/main/Lecture%205/assignment_outputs/Screenshot%20from%202025-01-21%2016-01-26.png)
   - Rename one of the columns in the data frame
     ```Python
     
        df.rename(columns={'Days' : 'No. of days'}, inplace=True)
     
     ```
     
     ![Output](https://github.com/mg270524/Data-Analytics-with-Python/blob/main/Lecture%205/assignment_outputs/Screenshot%20from%202025-01-21%2016-00-50.png)
     
   - Add an extra column
     ```Python
     
        df['No. of Mondays'] = [4,4,5,4,4,5,4,4,5,4,4,5]
     
     ```

     ![Output](https://github.com/mg270524/Data-Analytics-with-Python/blob/main/Lecture%205/assignment_outputs/Screenshot%20from%202025-01-21%2016-01-08.png)

1. Data Selection
   - All rows where a specific column has a value greater than a given number.
   - All columns where a specific column has a value greater than a given number.
   - A subset of columns
   - A specific row by its index

2. Missing value Treatments
   - Create a data frame with some missing values.
   - Identify the missing values
   - Replace the missing values with a fixed value, mean of a column, median of a column, interpolation
3. Grouping and Aggregation
   - Create a data frame with columns linke Branch, Students and CGPA
   - Group the data by branch and calculate
   - What more grouping can you do?
4. Merging and Joining (use help on pandas)
   - Create two data frames - one with student IDs and Names and another with IDs and CGPA
   - Merge the two data frames on students IDs
   - Perform different types of joins: inner, left and right
5. Handling time series data
   - DOwnload some stock data
   - Analyse this data
   - Create appropriate data
     
