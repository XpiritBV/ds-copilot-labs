# Lab 3: Titanic Dataset Lab: Exploratory Data Analysis (EDA)

This lab will guide you step-by-step through exploring, cleaning, visualizing, and modeling the Titanic dataset. Follow the prompts and tasks closely.

---


## Step 1: Ask Questions About the Data

Let’s return to our dataset and begin by developing an understanding of its contents.

### 🎯 Prompt (Ask Mode)

```
What do the columns sibsp and parch mean in the Titanic data?
```

**Task:**  Calculate and print the overall survival rate of passengers.

---

## 2. Clean Missing Values and Fix Data Types

Often, data contains missing values or incorrectly assigned data types. For example, if the `age` column has entries like `'?'`, pandas may set its type to `object` instead of a numeric type, which can interfere with calculations and visualizations.

**Step 1:**  
- Replace all `'?'` entries with `NaN` and ensure that numeric columns are properly typed.

**Step 2:**  
- Convert columns to numeric where possible. For instance, to prepare for correlation analysis, convert categorical variables to numbers (e.g., replace 'male' with 1 and 'female' with 0 in the `sex` column).


### 🎯 Prompt (Edit Mode)

```
Replace 'male' with 1 and 'female' with 0 in the sex column.
```

**Step 3:**  
- View the dataset to confirm these changes.

*Tip: Consider using data profiling tools such as Data Wrangler for interactive insights and transformations.*

---

## 3. Explore With Quick Visuals

With a clean dataset, use visualization libraries like seaborn and matplotlib to explore how various features relate to survival. Here are some ideas:

- **Survival Rate by Gender** (Bar Plot)
- **Age Distribution of Survivors vs. Non-survivors** (Histogram)
- **Survival Rate by Passenger Class** (Grouped Bar Plot)
- **Fare Distribution by Survival Status** (Boxplot)
- **Correlation Heatmap**


### 🎯 Prompt (Edit Mode)

```
Visualize the Age Distribution of Survivors and Non-survivors (Histogram) using seaborn and matplotlib.
```

Switch to Ask Mode:

Use the diagram as output to the chat (find the three dots in the top left of the diagram window):

![Output to chat example](images/Output%20to%20chat.png)

### 🎯 Prompt (Ask Mode)

```
Explain in plain English what this chart shows and highlight two surprising patterns.
```

**Task:** Change the style of the plot to your preference and observe how presentation impacts interpretation.

---

## 4. Analyze Correlations Between Input Variables

Let's calculate the correlations between all input variables and survival to identify which features might be useful for modeling. The closer the correlation is to 1 (or -1), the stronger the relationship.


### 🎯 Prompt (Ask Mode)

```
Show correlation of all numeric columns with Survived, sorted descending.
```

---

## 5. Finalize the Modeling DataFrame

With your correlation analysis done, retain only those fields that add significant signal to your model. Drop any columns with low value (such as `sibsp` and `parch`) and remove any remaining rows with missing values.

- Most likely, you will keep: `['Survived', 'Pclass', 'Sex', 'Age', 'Fare']`

*You can use Ask Mode for guidelines at this stage.*

---

## 6. Train and Evaluate a Model Using scikit-learn

Using your finalized DataFrame, train and evaluate a machine learning model (e.g., logistic regression) using scikit-learn.

**Tips:**  
- Use Ask Mode to draft a plan for implementation and explanation.
- Iterate on the plan as you go: refine, implement, evaluate, and explain.

---

## 7. Save the Trained Model

Once satisfied with your model, save it for use in the next lab:  
- File path: `../titanic_model.pkl`

---

Continue to the next steps or lab as instructed!

---

➡️ **[Next: Lab 4 Working with Copilot Instructions →](Lab%204%20Working%20with%20Copilot%20Instructions.md)**
