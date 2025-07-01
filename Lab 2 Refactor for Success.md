# Lab 2: Refactor for Success

## Refactoring Data Loading Logic

### Step 1: Download the Dataset

Download the Titanic dataset to your project folder:
[Titanic Dataset CSV](https://raw.githubusercontent.com/MicrosoftDocs/mslearn-introduction-to-machine-learning/main/Data/titanic.csv)

---

### Step 2: Refactor Data Loading (Edit Mode)


### 🎯 Prompt (Edit Mode)

```
Refactor the data loading logic in the notebook so that it is encapsulated in a function. This function should:
- Attempt to load the Titanic dataset from a local file in the data directory by default.
- If the local file does not exist, load the data from the provided URL.
- Move this function to a new Python file.
Be sure to follow best practices for code organization and reproducibility.
```

> **Why this prompt works well:**  
> This prompt is clear, specific, and actionable. It breaks down the task into concrete requirements (encapsulate logic in a function, handle both local and remote data sources, move to a new file, and follow best practices), which reduces ambiguity and makes it easy to implement and review. By specifying both the desired behavior and code organization, it encourages reproducibility—anyone following the prompt will produce a similar, maintainable solution.

---

### Step 3: Test the Code

Test the code after refactoring. Did it work? If not, try to fix the error using GitHub Copilot (Right-click → Copilot → Fix) or use the "Sparkles" icon next to the error.

---

### Step 4: Extract Configuration

Let's go further and extract the configurations:

Add both files as context (the function and the function call).


### 🎯 Prompt (Edit Mode)

```
Refactor the `load_titanic_data` function so that the default values for `local_path` and `url` are imported from a separate configuration module.
```

---

## Testing

Open the file with the `load_titanic_data` function.


### 🎯 Prompt (Agent Mode)

```
/tests load_titanic_data function and confirm that all tests pass successfully
```

---

### Explain Using Inline Chat

Browse through the generated code. Do you want an explanation of the created code? Select the code block, use inline chat (Ctrl + I), use the `/explain` command, or use the context menu (right-click → Copilot).

![Using inline chat in VS Code](images/inline%20chat.png)
*Use inline chat to quickly get explanations or suggestions for your code in VS

---

➡️ **[Next: Lab 3 EDA →](Lab%203%20EDA.md)**


