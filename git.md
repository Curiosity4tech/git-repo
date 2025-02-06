Here’s a simple **step-by-step guide** to contribute to an open-source project using GitHub and Git commands:

---

### 1. **Find a Repository to Contribute**
- Browse GitHub and select a project that interests you.
- Look for repositories with issues labeled as `good first issue`, `help wanted`, or `beginner-friendly`.

---

### 2. **Fork the Repository**
- On the repository page, click the **Fork** button (top-right corner). This creates a copy of the repository under your GitHub account.

---

### 3. **Clone Your Forked Repository**
- Copy the URL of your forked repository (from the **Code** button).
- Open your terminal and run:
  ```bash
  git clone <your-forked-repo-url>
  ```
- Navigate into the cloned directory:
  ```bash
  cd <repository-name>
  ```

---

### 4. **Set the Original Repository as Upstream**
- To keep your fork updated with the original repository, set it as `upstream`:
  ```bash
  git remote add upstream <original-repo-url>
  ```

- Verify remotes:
  ```bash
  git remote -v
  ```
  You should see:
  ```
  origin    <your-forked-repo-url> (fetch)
  upstream  <original-repo-url> (fetch)
  ```

---

### 5. **Create a New Branch**
- Always create a new branch for your changes:
  ```bash
  git checkout -b <branch-name>
  ```

---

### 6. **Make Changes**
- Edit files as needed. Use your favorite text editor or IDE.

---

### 7. **Stage and Commit Your Changes**
- Stage the changes:
  ```bash
  git add .
  ```
- Commit the changes with a descriptive message:
  ```bash
  git commit -m "Fix: Add feature or fix bug description"
  ```

---

### 8. **Push Your Branch to GitHub**
- Push your branch to your forked repository:
  ```bash
  git push -u origin <branch-name>
  ```

---

### 9. **Open a Pull Request (PR)**
- Go to the original repository on GitHub.
- You’ll see a button prompting you to **Compare & pull request**. Click it.
- Add a title and description explaining your changes, then submit the PR.

---

### 10. **Update Your Fork (Keep It in Sync)**
- If the original repository changes, update your fork:
  ```bash
  git checkout main
  git fetch upstream
  git merge upstream/main
  git push origin main
  ```

---

### 11. **Respond to Feedback**
- If maintainers suggest changes, update your branch locally:
  - Make changes.
  - Commit and push again:
    ```bash
    git push
    ```

---

### 12. **Celebrate Your Contribution! 🎉**
- Once your PR is merged, your contribution is officially part of the project!

Would you like more details on any specific step?