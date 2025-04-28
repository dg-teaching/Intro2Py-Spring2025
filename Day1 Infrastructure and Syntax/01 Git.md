# Git and VS Code Exercise: Neuroscience Data Analysis Project

## Introduction

In modern neuroscience research, collaboration and version control are essential. Whether you're analyzing complex brain imaging data or running computational models, you need efficient tools to manage your code, document your progress, and collaborate seamlessly with colleagues. **Visual Studio Code (VS Code)** is a powerful code editor that integrates well with **Git**, the world’s most popular version control system, and with **GitHub**, a platform for hosting and sharing code repositories.

In this exercise, you’ll learn some basic Git and GitHub workflows using VS Code—skills you can directly apply to a real-world neuroscience project.

---

## Part 1: Set Up Your Local Repository

### 1. Create a Blank Project in VS Code
1. Open Visual Studio Code.
2. From the **File** menu, select **Open Folder...** (or **Open...** on some systems).
3. Choose a new or empty folder where you’ll store your project files. 

*Short Description:* We’re setting up a dedicated space on your computer to keep all project files organized and ready for version control.

### 2. Create a `README.md`
1. In the **Explorer** sidebar (the left panel in VS Code), click **New File**.
2. Name the file `README.md`.

*Short Description:* The `README.md` file is where you’ll describe the purpose, usage, and any other relevant information about your project. Markdown (`.md`) files allow you to format text easily.

### 3. Add a Description Sentence
1. Open `README.md`.
2. Add a short description of your hypothetical data analysis project. For example:
```markdown
# Neuroscience Data Analysis Project
This project aims to analyze and visualize brain imaging data to identify patterns in neural activity.
```


3. Save the file (`File > Save` or **Ctrl+S** / **Cmd+S**).

*Short Description:* Giving a clear explanation of the project’s purpose can help other researchers quickly understand its goals and scope.

---

## Part 2: Initialize Git and Push to GitHub

### 4. Initialize a Local Git Repository
1. Open the **Source Control** panel in VS Code by clicking the Git icon (or press **Ctrl+Shift+G** / **Cmd+Shift+G**).
2. If your folder isn’t yet a Git repository, you will see an option to **Initialize Repository**. Click it.

*Short Description:* Initializing a local repo will allow you to track changes over time, roll back when needed, and collaborate with peers.

### 5. Stage and Commit Your `README.md`
1. In the **Source Control** panel, you should see `README.md` as a change.
2. Click the **+** icon next to `README.md` to stage it (or use the “Stage All Changes” option).
3. In the commit message box, type a brief message (e.g., `Add initial README.md`) and press **Enter** to commit.

*Short Description:* Staging files tells Git exactly which changes you want to include in your next snapshot (commit). Committing records those changes in the repo’s history.

### 6. Create a GitHub Repository and Push
1. Go to [GitHub.com](https://github.com/) and create a new **personal** repository. Name it (e.g., `neuroscience-data-analysis`).
2. Copy the repository’s URL (usually looks like `https://github.com/YourUserName/neuroscience-data-analysis.git`).
3. In VS Code, open the **Source Control** panel, click the three dots (menu), and select **Push to...**. If prompted to choose a remote, select `origin` or **Add Remote** and paste the GitHub URL.
4. After completing these steps, you should be able to push your local commits to GitHub.

*Short Description:* Pushing your code to GitHub stores it in a remote repository, enabling easy sharing and collaboration.

---

## Part 3: Forking and Collaborating

### 7. Fork Your Partner’s Repository
1. On GitHub, navigate to your partner’s repository.
2. Click the **Fork** button in the upper-right corner. 
3. This creates a personal copy of their repository under your GitHub account.

*Short Description:* Forking is a way to create your own copy of someone else’s repository, allowing you to propose changes without directly modifying their work.

### 8. Clone the Fork to VS Code
1. From your newly forked repository, click the **Code** button to copy the URL.
2. In VS Code, **Clone Git Repository** (using the **Source Control** panel or the Command Palette: **Ctrl+Shift+P** / **Cmd+Shift+P** → “Git: Clone”).
3. Paste the repository URL and choose a local folder for the clone.
4. Open the cloned folder in VS Code.

*Short Description:* Cloning means downloading the repository (and its entire version history) to your local machine so you can work on it.

### 9. Add Yourself to the "Contributors" Section
1. Open the `README.md` file in your local forked repository.
2. Add a new section, like:
   ```markdown
   ## Contributors
   - Your Name
   ```
3. Save the file.

*Short Description:* A **Contributors** section acknowledges people who have worked on the project, making it clear who did what.

### 10. Commit and Push Changes
1. Stage your changes in the **Source Control** panel by clicking the **+** next to `README.md`.
2. Write a commit message like `Add my name to Contributors section`.
3. Click the checkmark or press **Enter** to commit.
4. Push your changes to your fork on GitHub.

*Short Description:* Always write meaningful commit messages that clearly describe the changes you are making.

### 11. Open a Pull Request
1. Go to your forked repository on GitHub.
2. Click **Compare & pull request**.
3. Review the changes, make sure the base repository is your partner’s original repo, and the head repository is your fork.
4. Provide a descriptive title and message, then click **Create pull request**.

*Short Description:* A pull request notifies the original repository owner that you have proposed changes. They can review and merge your contributions into their project.

---

## Conclusion

By completing this exercise, you’ve practiced the essential steps for using **VS Code**, **Git**, and **GitHub** in a collaborative research environment—exactly what you’d do in a real neuroscience data analysis project. You learned how to:
- Initialize a local Git repository and create a `README.md`.
- Commit and push changes to a remote GitHub repository.
- Fork a partner’s repository, clone it locally, and contribute updates via a pull request.

This workflow keeps everyone on the same page and the project history well-documented. Happy coding and collaborating!
```
