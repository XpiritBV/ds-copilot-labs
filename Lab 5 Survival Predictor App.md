# Lab 5: Titanic Survival Predictor App (Agent Mode)

This lab will be heavily relying on the **Agent mode**: 

Let's build an interactive app that predicts survival outcomes for Titanic passengers using a trained model.

Create a Streamlit app (streamlit_app.py) that follow the requirements: 

1. **Model Loading**
   - Load a pre-trained logistic regression model (titanic_model.pkl) saved from a Jupyter notebook. Do not retrain the model in the app.
   - The model must be trained using the features: `Pclass`, `Sex`, `Age`, `Fare`

2. **Character Data Handling**
   - Load Titanic movie character data from a CSV (characters.csv) with columns: `Name`, `Pclass`, `Sex`, `Age`, `Fare`.In your prompt use #fetch https://en.wikipedia.org/wiki/Titanic_(1997_film) to load the characters from the movie
   - Allow users to add new characters interactively via input fields. Each new character should be appended to the CSV and reflected in the app.

3. **Prediction & Display**
   - For each character, predict survival probability using the loaded model.
   - Display a table with all characters, their features, predicted survival probability (as a percentage), and a human-readable explanation.

4. **Explanations**
   - Explanations must be detailed and reference the most important features for Titanic survival, based on correlation analysis (e.g., “Very likely to survive because she is a woman (women had the highest survival rate) and was in first class (first class passengers survived more often)”).
   - Explanations should be generated dynamically for each character, using their features and known Titanic survival patterns.

---

➡️ **[Next: Lab 6 Document →](Lab%206%20Document.md)**

