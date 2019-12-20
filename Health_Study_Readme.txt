The National Institute of Diabetes and Digestive and Kidney Diseases conducted a study on 768 adult female Pima Indians living near Phoenix

The dataset consist of the following columns:
        pregnant - numer of times the patient was pregnant
        glucose - plasma glucose concentration at 2 hours in an oral glocose tolerance test
        diagnostic - diastolic blood pressure (mm Hg)
        triceps - triceps skil fold thinkness (mm)
        insulin - 2-hour serum insulin (mu U/ml)
        bmi - body mass index (weigth in kg/height in meters squared)
        diabetes - diabetes pedigree function (a number representing genetic factors)
        age - client age in years (years)
        test - test whether patient shows signs of diabetes (0 if negative, 1 if positive)


Create a summary of the dataset. What is the mean insulin amount for patients in the study? What was the 3rd quartile of BMI? Check out the minimum values for glucose, diastolic BP, triceps, insulin and bmi - you don’t have to be a doctor to recognize that something is not quite right with these numbers. Please change them to NA so they don’t factor into the averages. Then summarize the data again note how the mean insulin and the 3rd quartile of BMI change.

Look at the test column… this column is set to 0 to indicate the patient does not have diabetes and 1 if they do. We prefer a “tidy” dataset, which means in part, we get rid of “coded” values. Let’s change the 0 to a “No”, and the 1 to a “Yes”. Then, recall our discussion of factors… let’s make this column a factor. Use the str() function to show that you have changed the test column into a factor. Now use the table function on the test column to determine how many in this dataset have diabetes.

Finally, let’s plot glucose against diastolic blood pressure (use the plot function). Do we get normal (or near normal) distributions? Finally, create a scatterplot of glucose against diastolic… do you see any kind of correlation? To see the correlation co-efficient you can use the cor function, just pass in the two columns. What is the co-efficient?