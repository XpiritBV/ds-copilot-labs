# Hands-on exercises: Titanic Survival Predictor with GitHub Copilot Chat

> **Goal**  
> Start from an empty repository and, through a series of hands-on steps, use GitHub Copilot Chat to scaffold, build, refactor, test, and ship an interactive model that predicts Titanic passenger survival chances.

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

## Next Step

➡️ [Start with Prerequisites](Prerequisites.md)
