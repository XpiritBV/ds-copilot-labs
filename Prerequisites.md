## Prerequisites

> **Note**: If you're using GitHub Codespaces, all prerequisites are automatically installed. These instructions are only for local development.

The following installations are required to complete these labs locally:

* [Visual Studio Code](https://code.visualstudio.com/)
* The [Python extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ms-python.python) and [Jupyter extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) (both published by Microsoft)
* [Miniconda with latest Python](https://docs.anaconda.com/miniconda/)
  * If you already have the full Anaconda distribution installed, you don't need to install Miniconda.
  * Alternatively, you can use a Python virtual environment and install the required packages with pip.

---

## Set up a Data Science Environment (Local Development Only)

> **Note**: Skip this section if you're using GitHub Codespaces - your environment is already configured!

Visual Studio Code and the Python extension provide a great editor for data science scenarios. With native support for Jupyter notebooks combined with Anaconda/Miniconda, it's easy to get started:

To create a Conda environment, open an Anaconda Prompt or terminal and run:

```sh
conda create -n myenv python=3.12 pandas jupyter seaborn scikit-learn matplotlib streamlit pytest
```

Or alternatively, create a virtual environment and install from requirements.txt:

```sh
python -m venv myenv
# On Windows:
myenv\Scripts\activate
# On macOS/Linux:
source myenv/bin/activate

pip install -r requirements.txt
```

For more info, see the [Anaconda documentation](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).

You are now ready to start your data science project in an isolated, reproducible environment!

---

## Version Control Best Practices (advice, but not necessary for the labs)

We recommend using a Git repository to store your code for all labs and exercises. Commit your changes often with clear messages. This makes it easy to revert to previous versions if needed and encourages good development habits when working with AI tools like GitHub Copilot.

---

➡️ **[Next: Lab 1: Project Setup and Intro to Copilot](./Lab%201%20Project%20Setup%20and%20Intro%20to%20Copilot.md)**