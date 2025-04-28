
# 🚀 Setup Instructions

Welcome! Follow these steps to get set up for the **Intro to Python** workshop.

---

## ✅ Quick Setup Checklist

- [ ] Clone the repository using **VSCode** (Source Control ➔ Clone Repository)
- [ ] Create the environment using **Pixi** (or **Conda**)
- [ ] Open and run the notebook `02 Checking it All Works.ipynb`

---

## 1. Clone the Repository (Using VSCode)

1. Open **Visual Studio Code**.
2. Click the **Source Control** icon (the branch symbol on the left sidebar).
3. Click **Clone Repository**.
4. Paste this URL:

   ```
   <your-repo-url>
   ```

5. Choose a folder where you want to save the project.
6. When prompted, **Open the repository** in a new window.

<sub>Tip: If you don't see "Source Control," press `Ctrl+Shift+P`, then search for "Git: Clone".</sub>

---

## 2. Create the Environment and Install Dependencies

You have two options:

### 🌟 Option 1: Using Pixi (Recommended)

If you have [Pixi](https://prefix.dev/docs/pixi/installation) installed:

```bash
pixi install
pixi shell
```

This will create and activate the environment automatically.

### 🛠️ Option 2: Using Conda

If you prefer Conda:

```bash
conda env create -f environment.yml
conda activate <your-environment-name>
```

<sub>Replace `<your-environment-name>` with the name specified inside `environment.yml`.</sub>

---

## 3. Open and Run the Notebook

1. In VSCode, open the file `02 Checking it All Works.ipynb`.
2. If prompted, install the **Python** and **Jupyter** extensions.
3. Press `Ctrl+Shift+P` ➔ Run **Python: Select Interpreter**.
4. Choose the environment you just created (Pixi or Conda).
5. Click **Run All** (at the top of the notebook) or run the cells one by one.

If everything is working, you're ready for the workshop!

---

# 📋 Reference Table

| Step                     | Tool             | Shortcut/Command                           |
|---------------------------|------------------|--------------------------------------------|
| Clone the repo            | VSCode Git GUI   | Source Control ➔ Clone Repository          |
| Open command palette      | VSCode           | `Ctrl+Shift+P`                             |
| Select Python environment | VSCode           | **Python: Select Interpreter**             |
| Create environment (Pixi) | Terminal         | `pixi install` + `pixi shell`              |
| Create environment (Conda)| Terminal         | `conda env create -f environment.yml`      |
| Open a notebook           | VSCode Explorer  | Open `02 Checking it All Works.ipynb`      |
| Run notebook cells        | VSCode Notebook  | Click **Run All** or use the play buttons  |

---

# 🛠️ Troubleshooting

Running into problems? Here’s what I recommend checking:

| Problem | What to try |
|:--------|:------------|
| **I can't see my environment in VSCode** | Open the Command Palette (`Ctrl+Shift+P`) ➔ Run **Python: Select Interpreter** ➔ pick the environment you created. |
| **VSCode says no Jupyter kernel found** | Make sure you have the **Jupyter** extension installed. If it’s already installed, try restarting VSCode. |
| **`pixi` or `conda` command isn’t recognized** | It might not be installed yet, or your terminal needs a restart. I recommend checking [Pixi installation](https://prefix.dev/docs/pixi/installation) or [Conda installation](https://docs.conda.io/en/latest/miniconda.html) if needed. |
| **I get errors when installing the environment** | Double-check that you're inside the folder you cloned. You can use `pwd` (Mac/Linux) or `cd` (Windows) to check. Also make sure the `pixi.toml` or `environment.yml` file is there. |
| **Git clone isn't working** | Git might not be installed yet. You can download it here: [git-scm.com](https://git-scm.com/). Let me know if you need help installing it. |
| **The notebook is open but running cells is super slow** | It could be using the wrong Python interpreter. Make sure you selected the environment you created using **Python: Select Interpreter**. |
| **I'm still stuck** | No worries — just ask me! I'm happy to help. 😊 |

