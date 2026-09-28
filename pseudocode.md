## pseudocode for assignment



Step 1:

load from a local csv source
  data -> read.csv("local_data")
  
  
  
Step 2:
Data cleansing:

does not = blank or null #Check for nulls
  run auto data type detection on all columns #Check data types
    if data %column% null then -> filtered data set  #Identify fully nulled columns, check them and ask why, then filter.
    
Step 3:

summary(data)
  calculate
    mean
    median
    average
    stdev on numeric types

Step 4:

  Run chart: (x,y) (numeric field, date field)
  Histogram: (x,y)  (test variable, count of observations)
  Data table: Pull descriptive text columns to filter on above observations

Step 5:
  Explain outlier variables from summary statistics, and null columns/missing data
  Extrapolate biggest drivers from the histogram and attempt to explain root cause
  Observe run chart and highlight increases in observation count, note the trend of the largest observation from the histogram (biggest driver)
  Summarize findings and recommend action based on cost drive
