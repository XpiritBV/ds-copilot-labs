Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

# Titanic Survival Predictor: A Hands-on Data Science Lab Series with GitHub Copilot

Welcome to the Titanic Survival Predictor labs! In this hands-on series, you’ll use GitHub Copilot in Visual Studio Code in the context of data science. 

Starting from scratch, you’ll work through labs covering data exploration, cleaning and modeling, and building an interactive prediction app. Along the way, you’ll learn to leverage Copilot Chat’s different modes (Ask, Edit, Agent) to speed up your workflow and follow best practices in data science

---

## Get to Know Copilot Chat — Modes at a Glance

| Mode | Best-for Tasks (lab-relevant examples) | Typical Actions & Example Prompts |
|------|----------------------------------------|-----------------------------------|
| **Ask** | • Explaining unfamiliar code blocks or ML concepts<br>• Clarifying dataset columns (e.g., `sibsp`, `parch`, `embarked`)<br>• Interpreting matplotlib/seaborn visualizations<br>• Understanding model performance metrics<br>• Getting data science best practices<br>• Troubleshooting errors and warnings | *"Explain what `sibsp` and `parch` columns represent in the Titanic dataset."*<br>*"Why is my correlation heatmap showing NaN values?"*<br>*"What's the difference between precision and recall for survival prediction?"*<br>*"How do I interpret this ROC curve?"*<br>*"What does this pandas warning about chained assignment mean?"* |
| **Edit** | • Refactoring notebook cells into reusable functions<br>• Adding proper error handling and validation<br>• Converting hardcoded values to configurable parameters<br>• Improving code with type hints and docstrings<br>• Optimizing pandas operations for performance<br>• Adding comprehensive unit tests | *"Move this data preprocessing code into a separate function with type hints."*<br>*"Add error handling for missing files and invalid data types."*<br>*"Refactor this plotting code into a reusable visualization function."*<br>*"Convert these magic numbers into named constants."*<br>*"Write pytest tests for the feature engineering functions."*<br>*"Optimize this loop using vectorized pandas operations."* |
| **Agent** | • Scaffolding complete project structure with best practices<br>• Generating full-featured Streamlit/Flask applications<br>• Creating comprehensive test suites and CI/CD pipelines<br>• Building multi-model comparison frameworks<br>• Setting up professional packaging (pyproject.toml, Docker)<br>• Generating documentation and deployment guides | *"Create a complete Streamlit app for Titanic survival prediction with file upload, model training, and interactive visualization."*<br>*"Generate a professional Python package structure with src/ layout, tests, and CI/CD configuration."*<br>*"Build a model comparison framework that trains and evaluates multiple algorithms (LogisticRegression, RandomForest, XGBoost)."*<br>*"Create a comprehensive test suite with unit tests, integration tests, and data validation tests."*<br>*"Set up a Docker containerized deployment with FastAPI backend and React frontend."* |

> **Tip – Mix & Match:**  
> • **Ask** for guidance → **Edit** to apply changes → **Agent** to scaffold whole features.  
> Switch modes fluidly as your task size grows.

## 📚 Useful Links

- [Prompt Engineering for Copilot Chat](https://docs.github.com/en/copilot/using-github-copilot/copilot-chat/prompt-engineering-for-copilot-chat)  
  *How to write effective prompts*

- [Prompting Guide](https://www.promptingguide.ai/)  
  *A helpful guide for crafting effective prompts for AI tools like GitHub Copilot*

- [GitHub Copilot Chat Cheat Sheet](https://docs.github.com/en/copilot/using-github-copilot/copilot-chat/github-copilot-chat-cheat-sheet?tool=vscode)  
  *Commands and best practices (or simply use `/help` in chat!)*

- [Which AI Model Should I Use with Copilot?](https://github.blog/ai-and-ml/github-copilot/which-ai-model-should-i-use-with-github-copilot/)  
  *AI model selection guide*

---

## Getting Started

### Option 1: GitHub Codespaces (Recommended)

The easiest way to get started is using GitHub Codespaces with the included devcontainer configuration:

1. Click the **Code** button on the GitHub repository
2. Select **Codespaces** tab
3. Click **Create codespace on main**
4. Wait for the environment to set up automatically

The devcontainer includes:
- Python 3.11 with all required data science packages
- VS Code with Python, Jupyter, and GitHub Copilot extensions
- Pre-configured environment ready for the labs

### Option 2: Local Setup

If you prefer to work locally, follow the instructions in [Prerequisites](./Prerequisites.md).

---

## Lab Sequence

- [Prerequisites](./Prerequisites.md)
- [Lab 1: Project Setup and Intro to Copilot](./Lab%201%20Project%20Setup%20and%20Intro%20to%20Copilot.md)
- [Lab 2: Refactor for Success](./Lab%202%20Refactor%20for%20Success.md)
- [Lab 3: Light EDA](./Lab%203%20EDA.md)
- [Lab 4: Working with Copilot Instructions](./Lab%204%20Working%20with%20Copilot%20Instructions.md)
- [Lab 5: Build Survival Predictor App in Agent Mode](./Lab%205%20Survival%20Predictor%20App.md)
- [Lab 6: Project Documentation](./Lab%206%20Document.md)





