# Exercise 6: Weather data calculation

The aim of this exercise is to analyze historical weather data. In Problem 1 you read in a tricky data file and explore it's contents. In problem 2, you will convert and aggregate the data from daily temperatures in Fahrenheit, to monthly average temperatures in Celsius. 

**Notice**: Closely follow the instructions! Please use **exactly** the same variable names mentioned in the instructions because your answers will be automatically graded, and the tests that grade your answers rely on following the given variable naming. 


## Problem 1 - Reading in a tricky data file 

You first task for this exercise is to read in the data file [data/1091402.txt](data/1091402.txt) to a variable called `data`. Pay attention to the input data structure and no data values.

**Your score on this problem will be based on following criteria:**

- Reading the data into a variable called `data` using Pandas
    - Skipping the second row of the datafile that contains `----------` characters that don't belong to the data
    - Convert the no-data values (`-9999`) into `NaN` 
- Calculating basic statistics from the data
- Including comments that explain what most lines in the code do

### Part 1

You should start by reading the data file.

- Read the data file into variable the variable `data`
    - Skip the second row
    - Convert the no-data values (`-9999`) into `NaN`


```python
!pip install pandas
!pip install numpy
```


```python
import pandas as pd
import numpy as np
```


```python
data = None

# YOUR CODE HERE 1
```


```python
# Check that the dataframe looks ok:
data.head()
```


```python
# Check the last rows of the data (there should be some NaN values)
data.tail()
```

### Part 2 

In this section, you will calculate simple statistics based on the input data:

- Calculate how many no-data (NaN) values there are in the `TAVG` column
    - Assign your answer to a variable called `tavg_nodata_count`.


```python
tavg_nodata_count = None
#YOUR CODE HERE 2
```


```python
# Print out the solution:
print('Number of no-data values in column "TAVG":',tavg_nodata_count)
```

- Calculate how many no-data (NaN) values there are for the `TMIN` column
    - Assign your answer into a variable called `tmin_nodata_count`


```python
tmin_nodata_count = None
#YOUR CODE HERE 3
```


```python
# Print out the solution:
print('Number of no-data values in column "TMIN":', tmin_nodata_count)
```

- Calculate the total number of days covered by this data file

    - Assign your answer into a variable called day_count


```python
day_count = None 
#YOUR CODE HERE 4
```


```python
# Print out the solution:
print("Number of days:", day_count)
```

- Find the date of the oldest (first) observation
    - Assign your answer into a variable called `first_obs`


```python
first_obs = None
 
# YOUR CODE HERE 5
```


```python
# Print out the solution:
print('Date of the first observation:',first_obs)
```

- Find the date of the most recent (last) observation
    - Assign your answer into a variable called `last_obs`


```python
last_obs = None

# YOUR CODE HERE 6
```


```python
# Print out the solution:
print('Date of the last observation:', last_obs)
```

- Find the average temperature for the whole data file (all observtions) from column `TAVG`
    - Assign your answer into a variable called `avg_temp`


```python
avg_temp = None

# YOUR CODE HERE 7
```


```python
# Print out the solution:
print('Average temperature (F) for the whole dataset:', round(avg_temp, 2))
```

- Find the average `TMAX` temperature over the Summer of 1969 (months May, June, July, and August of the year 1969)
    - Assign your answer into a variable called `avg_temp_1969`


```python
avg_temp_1969 = None

# YOUR CODE HERE 8
```


```python
# This test print should print a number
print('Average temperature (F) for the Summer of 69:', round(avg_temp_1969, 2))
```

## Problem 2 - Calculating monthly average temperatures

For this problem your goal is to calculate monthly average temperatures in degrees Celsius from the daily Fahrenheit values we have in the data file. You can continue working with the same DataFrame that you used in Problem 1.

**Your score on this problem will be based on following criteria:**

- Calculating the monthly average temperatures in degrees Celsius for the each month in the dataset (i.e., for each month of each year)
    - You should store the monthly average temperatures in a new Pandas DataFrame called `monthly_data`
    - `monthly_data` should contain a new column called `temp_celsius` the monthly average temperatures in Celsius
    - Convert the `TAVG` values in Fahrenheit into Celsius and store the output in the `temp_celsius`
- Including comments that explain what most lines in the code do
- Uploading your notebook to your GitHub repository for this week's exercise

*Hint: you can start by creating a new column with a label for each month and then continue grouping the data based on this information.*


```python
monthly_data = None

# YOUR CODE HERE 9
```


```python
# This test print should print the length of variable monthly_data
print(len(monthly_data))
```


```python
# This test print should print the column names of monthly_data
print(monthly_data.columns.values)
```


```python
# This test print should print the mean of temp_celsius
print(round(monthly_data['temp_celsius'].mean(),2))
```


```python
# This test print should print the median of temp_celsius
print(round(monthly_data['temp_celsius'].median(), 2))
```


