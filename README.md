# Neural-Network-Assignment-ICP_3

NAME: RAMA KRISHNA GANTA ID#: 700759560

1. Data Manipulation
   
      a.	Read the provided CSV file ‘data.csv’.
   
      b.	https://drive.google.com/drive/folders/1h8C3mLsso-R-sIOLsvoYwPLzy2fJ4IOF?usp=sharing
   
      c.	Show the basic statistical description about the data.
   
      d.	Check if the data has null values.
   
      i.	Replace the null values with the mean
   
      e.	Select at least two columns and aggregate the data using: min, max, count, mean.
   
      f.	Filter the dataframe to select the rows with calories values between 500 and 1000.
   
      g.	Filter the dataframe to select the rows with calories values > 500 and pulse < 100.
   
      h.	Create a new “df_modified” dataframe that contains all the columns from df except for “Maxpulse”.
   
      i.	Delete the “Maxpulse” column from the main df dataframe.
   
      j.	Convert the datatype of Calories column to int datatype.
   
      k.	Using pandas create a scatter plot for the two columns (Duration and Calories).
  	
Solution:
          It begins by uploading a CSV file from your local system using files.upload() and then reads the file into a pandas DataFrame. Basic statistical descriptions of the data are generated using the describe() method, followed by a check for null values. Any missing values are replaced with the mean of their respective columns using fillna(). The script then aggregates data from two specific columns, 'Calories' and 'Pulse', by calculating their minimum, maximum, count, and mean values.

Next, the script filters the data based on conditions: rows where Calories is between 500 and 1000, and rows where Calories is greater than 500 and Pulse is less than 100. Additionally, the code removes the 'Maxpulse' column from both a new DataFrame (df_modified) and the original DataFrame, while converting the Calories column to an integer data type. Finally, it creates a scatter plot to visualize the relationship between Duration and Calories, using matplotlib. The results of each operation, including statistical summaries, filtered data, and the scatter plot, are displayed in the notebook.

Output:

Basic Statistical Description:
          Duration       Pulse    Maxpulse     Calories
count  169.000000  169.000000  169.000000   164.000000
mean    63.846154  107.461538  134.047337   375.790244
std     42.299949   14.510259   16.450434   266.379919
min     15.000000   80.000000  100.000000    50.300000
25%     45.000000  100.000000  124.000000   250.925000
50%     60.000000  105.000000  131.000000   318.600000
75%     60.000000  111.000000  141.000000   387.600000
max    300.000000  159.000000  184.000000  1860.400000

Null Values in each column:
 Duration    0
Pulse       0
Maxpulse    0
Calories    5
dtype: int64

Null values replaced with mean.

Aggregated Data:
           Calories       Pulse
min      50.300000   80.000000
max    1860.400000  159.000000
count   169.000000  169.000000
mean    375.790244  107.461538

Rows with Calories between 500 and 1000:
      Duration  Pulse  Maxpulse  Calories
51         80    123       146     643.1
62        160    109       135     853.0
65        180     90       130     800.4
66        150    105       135     873.4
67        150    107       130     816.0
72         90    100       127     700.0
73        150     97       127     953.2
75         90     98       125     563.2
78        120    100       130     500.4
83        120    100       130     500.0
90        180    101       127     600.1
99         90     93       124     604.1
101        90     90       110     500.0
102        90     90       100     500.0
103        90     90       100     500.4
106       180     90       120     800.3
108        90     90       120     500.3

Rows with Calories > 500 and Pulse < 100:
      Duration  Pulse  Maxpulse  Calories
65        180     90       130     800.4
70        150     97       129    1115.0
73        150     97       127     953.2
75         90     98       125     563.2
99         90     93       124     604.1
103        90     90       100     500.4
106       180     90       120     800.3
108        90     90       120     500.3

New dataframe 'df_modified' without 'Maxpulse' column:
    Duration  Pulse  Calories
0        60    110     409.1
1        60    117     479.0
2        60    103     340.0
3        45    109     282.4
4        45    117     406.0

'Maxpulse' column deleted from original dataframe.

Calories column datatype converted to int.

![download](https://github.com/user-attachments/assets/cacf6186-df71-4634-a32e-6e89eb46b3b1)

2.	Linear Regression
    a)	Import the given “Salary_Data.csv”
  	
    b)	Split the data in train_test partitions, such that 1/3 of the data is reserved as test subset.
  	
    c)	Train and predict the model.
  	
    d)	Calculate the mean_squared error
  	
    e)	Visualize both train and test data using scatter plot.

Solution:
          This Python script, performs linear regression analysis on a dataset that is uploaded via the Colab interface. The script begins by importing necessary libraries including pandas for data manipulation, matplotlib for plotting, and sklearn for machine learning tasks. After uploading the dataset, it loads the data into a DataFrame and splits it into training and testing sets, with one-third of the data reserved for testing. The script then initializes and trains a linear regression model using the training data.

The model is used to make predictions on both the training and testing sets. The Mean Squared Error (MSE) of the predictions on the test set is calculated and printed to evaluate model performance. Finally, the script visualizes the results by plotting scatter plots of both the training and test data, along with their respective regression lines. The plots are displayed with different colors to distinguish between training and test data, helping to visualize the relationship between years of experience and salary, as well as the model's fit to the data.

Output:


![download](https://github.com/user-attachments/assets/9eb40d41-d897-40d7-bb5c-5b7ca685d170)





