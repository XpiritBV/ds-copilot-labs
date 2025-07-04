## Prerequisites

> **Note**: If you're using GitHub Codespaces, all prerequisites are automatically installed. These instructions are only for local development.

The following installations are required to complete these labs locally:

* [Visual Studio Code](https://code.visualstudio.com/)
* [Python](https://www.python.org/downloads/) (latest version recommended)
* The [Python extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ms-python.python) and [Jupyter extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) (both published by Microsoft)
---

## Set up a Data Science Environment (Local Development Only)

> **Note**: Skip this section if you're using GitHub Codespaces - your environment is already configured!

Setting up a Python virtual environment is **strongly recommended** as a best practice for Python projects to avoid dependency conflicts.

### 1. Download Dependencies File

Download the [`requirements.txt`](requirements.txt) file and save it to your project folder.

### 2. Set Up Virtual Environment

> **Important**: Ensure your terminal is open in the **same directory as `requirements.txt`** before running these commands.

#### Windows:
```cmd
python -m venv dslab
dslab\Scripts\activate
pip install -r requirements.txt
```

#### macOS/Linux:
```bash
python -m venv dslab
source dslab/bin/activate
pip install -r requirements.txt
```

### 3. Verify Installation

You can verify your environment is set up correctly by running:
```cmd
pip list
```

You are now ready to start your data science project in an isolated, reproducible environment!

---

## Version Control Best Practices (advice, but not necessary for the labs)

We recommend using a Git repository to store your code for all labs and exercises. Commit your changes often with clear messages. This makes it easy to revert to previous versions if needed and encourages good development habits when working with AI tools like GitHub Copilot.

---

➡️ **[Next: Lab 1: Project Setup and Intro to Copilot](./Lab%201%20Project%20Setup%20and%20Intro%20to%20Copilot.md)**