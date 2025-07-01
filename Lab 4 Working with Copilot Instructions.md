# Lab 4: Working with GitHub Copilot Custom Instructions

In this lab, you will learn how to use GitHub Copilot Custom Instructions to standardize the style of your plots across your Python project. Custom instructions let you define preferences for how Copilot suggests code, making your workflow more consistent and tailored to your needs.

---

## 1. Example: Custom Instructions Markdown File

Below is an example of a custom instructions file (`.github/copilot-instructions.md`) that applies to all Python (`.py`) and Jupyter Notebook (`.ipynb`) files in your project:

```markdown
---
applyTo:
  - "**/*.ipynb"
  - "**/*.py"
---

**Plotting style**  
  • Prefer seaborn and matplotlib for plots; set a gentle pastel palette.  
  • When plotting, rotate x-tick labels 45° for readability.
```

---

## 2. Test the Instruction in Action

Let's plot a histogram using your custom instructions.

### 🎯 Prompt (Edit Mode)

```
Plot Age Distribution of Survivors and Non-survivors (Histogram)
```

See if your custom instructions were applied.

---

**Experiment:**  
Think about your use case and try to change the instruction file. Observe how Copilot's suggestions adapt.

---

**Tip:**  
These custom instructions will be global for your project. For specialized instructions, you can create an instruction file in the `.github/instructions` folder.

More about custom instructions:  
[Copilot Customization Documentation](https://code.visualstudio.com/docs/copilot/copilot-customization)

---

➡️ **[Next: Lab 5 Survival Predictor App →](Lab%205%20Survival%20Predictor%20App.md)**


