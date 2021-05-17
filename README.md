# Exercise 6 - Data analysis with Pandas

In this week's exercise we will continue developing our skills using Pandas to analyze climate data.

The aim of this exercise is to analyze historical weather data and weather anomalies. In Problem 1 you read in a tricky data file and explore it's contents. In problem 2, you will convert and aggregate the data from daily temperatures in Fahrenheit, to monthly average temperatures in Celsius. 
- **Exercise 6 is due by the start of the next lesson (9:00 am, 24 May 2021)**.

## Input data
For problems 1-3 in this exercise we will be using historical climate data from the Helsinki-Vantaa airport station. For these problems, we have daily observations obtained from the NOAA Global Historical Climatology Network. The file was downloaded using the "Custom GHCN-Daily Text" output format, including following attributes:

| Attribute                | Description                      |
|--------------------------|----------------------------------|
| `STATION`                | Unique ID of the weather station |
| `ELEVATION`              | Elevation of the station         |
| `LATITUDE` , `LONGITUDE` | Coordinates of the station       |
| `DATE`                   | Date of the measurement          |
| `PRCP`                   | Precipitation                    |
| `TAVG`                   | Average temperature              |
| `TMAX`                   | Maximum temperature              |
| `TMIN`                   | Minimum temperature              |

Note: once again that temperatures in this dataset are given in degrees Fahrenheit.

## Getting started

- Before starting, run 

```Shell
pip install pandas
```

in the Repl.it shell. In the right panel of the repl.it page, you see "Console", "Shell", and "Markdown" tabs. Click the "Shell" tab, and input 
```Shell
pip install pandas
```
and hit enter key. Then, the installation of pandas starts. Wait a moment until it finishes the installation.

Always fill in the parts saying YOUR CODE HERE:
```
# YOUR CODE HERE 1
```
You have nine parts in this assignment.

### Parts you should not edit
Please don't edit the parts between the lines : 

#CAUTION!!! DON'T EDIT THIS PART START

and

#CAUTION!!! DON'T EDIT THIS PART END

These lines are for autograding.  If you edit these lines, the instructor cannot evaluate your work correctly.

```
#CAUTION!!! DON'T EDIT THIS PART START
# ... Please don't edit this line 1
# ... Please don't edit this line 2
#CAUTION!!! DON'T EDIT THIS PART END
```
