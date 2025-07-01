1. Open VS code. Let's start from the scratch
Navigate to Github copilot chat. Enter /help - take a look at the available build in helper commands - you will experiment with them very shortly! 

## 1  Project Bootstrap and reading the data (Agent)
2. Let's create our project. For the data exploration we are going to use dataset: https://raw.githubusercontent.com/MicrosoftDocs/mslearn-introduction-to-machine-learning/main/Data/titanic.csv 

prompt: 

/new Create a new Python data science project to analyze Titanic survival data.  
- Scaffold the project structure following Python data science best practices.
- Add a Jupyter notebook to the project.
- In the notebook, include code to read the Titanic dataset from:  
  `https://raw.githubusercontent.com/MicrosoftDocs/mslearn-introduction-to-machine-learning/main/Data/titanic.csv`

note: use the enviroment created in Prerequisites. 

Questions:
Did it generate the structure you expected? You can iterate changing the prompt or with follow up commands in the chat. 

Use "Ask" mode to find out best practices for Project Bootstrap for data science using Python. 
prompt: 

**"What are the recommended best practices for setting up (bootstrapping) a new data science project using Python and Jupyter notebooks?"**


## 2 Refactor (Edit mode)

Download dataset https://raw.githubusercontent.com/MicrosoftDocs/mslearn-introduction-to-machine-learning/main/Data/titanic.cs to the project folder. 

Prompt: 
Refactor the data loading logic in the notebook so that it is encapsulated in a function. This function should:

- Attempt to load the Titanic dataset from a local file in the data directory by default.
- If the local file does not exist, load the data from the provided URL.
- Move this function to a new Python file
Be sure to follow best practices for code organization and reproducibility.


Test the code. 
Did it work? If not, try to fix the error using GitHub Copilot (Right click -> Copilot-> Fix or using "Sparkles" icon nexr to the error). 

Let's go further and extract the configurations: 
Add both files as a context (the functuon adn function call): 

Prompt: 
Refactor the `load_titanic_data` function so that the default values for `local_path` and `url` are imported from a separate configuration module

## Tests (Agent mode)

Open the file with load_titanic_data function

prompt: 
/tests load_titanic_data function and confirm that all tests pass successfully

### Expalin using inline chat: 

Browse through the generated code. Do you want and explanation of the created code? Select the code block, use inline chat(Ctrl + i) use /explain command or context menu (righ click -> Copilot) 


Tip: maybe you worked with Copilot before? Now you hvae time to experiment with different models: https://docs.github.com/en/copilot/reference/ai-models/choosing-the-right-ai-model-for-your-task 
You can go a step further: describe your task and ask github copilt to suggest you models providing a link to the documentation with #fetch https://docs.github.com/en/copilot/reference/ai-models/choosing-the-right-ai-model-for-your-task 