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





