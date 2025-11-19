Thank you for contributing to this repository!
This guide outlines the standard process for submitting **Issues** and **Pull Requests (PRs)** to ensure smooth collaboration and consistent quality.

---

## 📌 Table of Contents
- [Submitting Issues](#-submitting-issues)
- [Contributing via Pull Requests](#-contributing-via-pull-requests)
  - [1. Fork the Repository](#1-fork-the-repository)
  - [2. Set Up Development Environment](#2-set-up-development-environment)
  - [3. Create a Branch](#3-create-a-branch)
  - [4. Make Changes and Commit](#4-make-changes-and-commit)
  - [5. Push to Your Fork](#5-push-to-your-fork)
  - [6. Create a Pull Request](#6-create-a-pull-request)
  - [7. Pass Continuous Integration (CI)](#7-pass-continuous-integration-ci)
  - [8. Address Review Comments](#8-address-review-comments)

---

## 🐞 Submitting Issues

Issues help track **bugs**, **feature requests**, and **documentation improvements**.

Please review existing issues before creating a new one.

### **Issue Categories**

#### 1. Bug Reports
- Describe the issue clearly, including **steps to reproduce**, **expected**, and **actual results**.
- Provide **environment details** (e.g., OS, Python, MindSpore version).
- Attach **logs or screenshots** if available.

#### 2. Feature Requests
- Explain the motivation and expected benefit.
- Add examples or usage scenarios if possible.

#### 3. Documentation Improvements
- Specify the section or file needing updates.
- Suggest clear edits or additions.

#### 4. Other Topics
- For discussions or questions, state the goal and provide enough context.

> 💡 **Tip:** Always use the Issue Template if provided, and fill in all required fields for clarity.

---

## 🧩 Contributing via Pull Requests

All code or documentation changes should go through PRs.
Follow the steps below for a clean and reviewable contribution process.

---

### **1. Fork the Repository**
- On GitHub: click "Fork" on the top right.
- Clone your fork and add upstream:

```bash
git clone git@github.com:your-username/repo-name.git
cd repo-name
git remote add upstream git@github.com:original-owner/repo-name.git
# Check all the remote repositories
git remote -v
```

### **2. Set Up Development Environment**

Install required dependencies:

```bash
pip install -r requirements.txt
```

> For users in limited network regions, check the alternative setup guide (via Docker image) if available.

### **3. Create a Branch**

Use a descriptive branch name:
```bash
git checkout -b [prefix]/short-description
```

**Here are some recommended refix options for reference:**

- `feature/` – new feature
- `fix/` – bug fix
- `docs/` – documentation changes
- `wip/` – work in progress

### **4. Make Changes and Commit**

- Run all unit tests locally.
- Perform linting and style checks using the same tools defined in the CI pipeline.
- Confirm all tests pass before committing any changes.
- Commit changes with a clear message:

```bash
git add .
git commit -m "[Prefix] Brief description of changes"
```

### **5. Push to Your Fork**
```bash
git push origin [your-branch-name]
```

### **6. Create a Pull Request**

- On the original repository, click “Compare & pull request.”
- Fill in the PR template:
```text
Title: [Prefix] Short summary
Description: Explain the purpose, approach, and related issue (e.g., Fixes #123).
Testing: Include key tests or verification steps.
```

### **7. Pass Continuous Integration (CI)**

- All PRs trigger automated CI tests (unit tests, lint checks, etc.).
- Monitor the **PR Checks** panel. If any test fails, click **Details**, fix the issue, and re-push.
- Only PRs passing all CI checks can be merged.

### **8. Address Review Comments**

- Respond promptly to reviewer feedback.
- Commit updates based on comments and push again.
- The PR will auto-update for re-review.

Once approved, a committer will merge your PR.
🎉 Thank you for making this project better!