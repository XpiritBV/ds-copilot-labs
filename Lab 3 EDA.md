### EDA

## 2 Ask questions about notebook content (Ask mode)
Back to our dataset!

Fox example you can start asking question about the data. 

Prompt: “What do the columns sibsp and parch mean in Titanic data?”

Task: 
Calculate and print survival rate

## 2 Clean missing values and fix dtypes

While Pandas can read this value into a DataFrame, the result for a column like age is that its data type will be set to object instead of a numeric data type, which is problematic for graphing.

This problem can be corrected by replacing the question mark with a missing value that pandas is able to understand. 

1. Task: Replaces `'?'` with `NaN` and ensure numeric columns are truly numeric

In future steps we would like to calculate correlations. To do so, all the variables used need to be numeric for the correlation calculation and fopr example currently gender is stored as a string

2. Task: Convert columns to numeric where possible (Prompt: Replace 'male' with 1 and 'female' with 0 in the sex column.)

3. View the dataset to confirm the chnages:

Tip: you can use the data viewing experience offered by other extensions like Data Wrangler. The Data Wrangler extension offers a rich user interface to show insights about your data and helps you perform data profiling, quality checks, transformations, and more. 

## Explore with quick visuals
Now that the data is in good shape, you can use seaborn and matplotlib to view how certain columns of the dataset relate to survivability. 

Here are some ideas for vizualizing:

Survival Rate by Gender (Bar Plot)
Age Distribution of Survivors and Non-survivors (Histogram)
Survival Rate by Passenger Class (Grouped Bar Plot)
Fare Distribution by Survival Status (Boxplot)
Correlation Heatmap

Example (Edit mode): 
Prompt: Vizualize Age Distribution of Survivors and Non-survivors (Histogram) using seaborn and matplotlib

Go to Ask Mode:

USe the diagram as an output to chat (three dots on the left top of diagram):

![Output to chat example](images/Output%20to%20chat.png)

Prompt: 
Explain in plain English what this chart shows; highlight two surprising patterns. 

Task:
Ask to change the style of the plot according to your taste :) 


### Analyze the correlation between all the input variables

#### Encode Categorical Features.

These graphs are helpful in seeing some of the relationships between survival and the input variables of the data, but it's also possible to use pandas to calculate correlations. To do so, all the variables used need to be numeric for the correlation calculation and currently gender is stored as a string. We need to convert those string values to integers. 

Many algorithms expect numerical input. Convert sex from strings to a binary indicator (1 = male, 0 = female).

Prompt: Replace 'male' with 1 and 'female' with 0 in the sex column.

Now, you can analyze the correlation between all the input variables to identify the features that would be the best inputs to a machine learning model. The closer a value is to 1, the higher the correlation between the value and the result. Use the following code to correlate the relationship between all variables and survival.

Prompt:
Show correlation of all numeric columns with survived, sorted descending.

### Finalize the Modeling DataFrame
Keep the fields that add signal, drop the rest, and remove any remaining rows with missing values.

With this information in hand, you can now drop from the dataset the low value sibsp and parch columns, as well as any rows that had NaN values, to end up with a dataset that can be used for training a model.

You can use Ask mode for the the guildlines. 

most likely you will end up with ['Survived', 'Pclass', 'Sex', 'Age', 'Fare'] 

### Train and evaluate a model using scikit-learn

With your finall dataframe train and evaluate the model. 
Tip: you combination of modes, start with Ask mode asking for the plan of implemnentation and explanation. Iterate on the plan,  

### Save the trained model for use in the next lab ("../titanic_model.pkl")

























