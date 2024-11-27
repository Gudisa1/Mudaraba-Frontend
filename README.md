---
# Team Collaboration Guidelines

Welcome to the repository! This document provides essential guidelines for contributing, committing, and collaborating effectively.
---

## 📂 **Branching Strategy**

1. **Main Branch**:

   - The `main` branch is **protected** and always reflects production-ready code.
   - Direct pushes to `main` are not allowed. Use Pull Requests (PRs) to merge changes.

2. **Feature Branches**:

   - Create a feature branch for any new feature or fix.
   - Name the branch descriptively:
     - **Features**: `feature/your-feature-name`
     - **Bugs**: `bugfix/issue-description`
     - **Hotfixes**: `hotfix/critical-fix`
   - Example:
     ```bash
     git checkout -b feature/add-login-functionality
     ```

3. **Branch Workflow**:
   - Always pull the latest changes from `main` before starting your work:
     ```bash
     git checkout main
     git pull origin main
     ```
   - Regularly sync your branch with `main` to resolve conflicts early.

---

## ✏️ **Commit Guidelines**

1. Write clear, concise commit messages:

   - **Format**: `<type>(<scope>): <description>`
   - **Examples**:
     - `feat(auth): add user login functionality`
     - `fix(ui): resolve alignment issues on navbar`
     - `docs(readme): update contribution guidelines`

2. **Types of Commits**:
   - `feat`: Adding a new feature
   - `fix`: Fixing a bug
   - `docs`: Documentation changes
   - `style`: Code style changes (e.g., formatting, indentation)
   - `refactor`: Code refactoring without changing functionality
   - `test`: Adding or updating tests

---

## 📤 **Pushing Changes**

1. Stage your changes:
   ```bash
   git add .
   ```
2. Commit your changes:
   ```bash
   git commit -m "feat(auth): add user login functionality"
   ```
3. Push your branch to the remote repository:
   ```bash
   git push origin feature/add-login-functionality
   ```

---

## ✅ **Pull Requests (PRs)**

1. **Creating a Pull Request**:

   - Always create a PR to merge your branch into `main`.
   - Add a clear title and description for your PR:
     - **Title**: `[Feature] Add Login Functionality`
     - **Description**: Explain the purpose, changes made, and testing steps.

2. **Code Reviews**:

   - Ensure all tests pass before requesting a review.
   - At least **one reviewer** must approve the PR before merging.
   - Be open to constructive feedback.

3. **Merging**:
   - Do not merge your own PR unless explicitly permitted.
   - Use **Squash and Merge** to maintain a clean commit history.

---

## 🧪 **Testing**

1. Write or update tests for your changes.
2. Run tests locally before pushing:
   ```bash
   npm test
   ```

---

## 📜 **Code of Conduct**

1. Be respectful in all communications.
2. Adhere to clean coding practices and team standards.
3. Commit only your work. Avoid pushing temporary files, secrets, or personal configurations.

---

## 🛠️ **Setup and Development**

1. Clone the repository:
   ```bash
   git clone https://github.com/<organization>/<repo-name>.git
   cd <repo-name>
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Run the development server:
   ```bash
   npm run dev
   ```

---

## 🚀 **Deployment Workflow**

- Deployment to production occurs from the `main` branch.
- Tag releases using semantic versioning:
  ```bash
  git tag -a v1.0.0 -m "Release version 1.0.0"
  git push origin v1.0.0
  ```

---

By following these guidelines, we can ensure smooth collaboration, maintain code quality, and build great features together! 🎉

---
