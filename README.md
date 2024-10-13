# predict_price_of_car_used
 ## Loading the raw data
   # Load the data from a .csv in the same folder using Pandas
 ## Preprocessing
 ### Determining the variables of interest
     we will create the regression without 'Model'
 ### Dealing with missing values
    # data.isnull() # shows a df with the information whether a data point is null 
 ### Exploring the PDFs
      #The PDF will show us how that variable is distributed 
      his makes it very easy to spot anomalies, such as outliers
 ### Dealing with outliers
   #Outliers are a great issue for OLS, thus we must deal with them in some way
 ## Checking the OLS assumptions
 ### Relaxing the assumptions
    # Let's transform 'Price' with a log transformation
 ### Multicollinearity
  # Since Year has the highest VIF, I will remove it from the model
  # This will drive the VIF of other variables down!!! 
 ## Linear regression model
      ### Scale the data
  ### Train Test Split
    # I am Split the variables with an 80-20 split and some random state
