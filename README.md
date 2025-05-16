# DevOps Git Project

## 📌 Objective

This project demonstrates how to manage a DevOps project using Git and GitHub following best version control practices. It focuses on proper branching, pull request workflows, tagging, and documentation.

---

## 🛠 Tools Used

- **Git**: Distributed version control system.
- **GitHub**: Remote repository hosting and collaboration.
- **Markdown**: For documentation and task tracking.

---

## 🗂 Branching Strategy

| Branch        | Purpose                                  |
|---------------|-------------------------------------------|
| `main`        | Production-ready code                     |
| `dev`         | Active development and testing            |
| `feature/*`   | New features, fixes, or enhancements      |

**Workflow:**
- Feature branches are created from `dev`.
- Pull requests (PRs) are used to merge `feature/*` into `dev`.
- Once tested and verified, `dev` is merged into `main` via PR.

---

## 🔁 Git Workflow Summary

1. Clone repo and create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   
2.Commit and push changes:

bash
Copy
Edit
git add .
git commit -m "Describe your change"
git push origin feature/your-feature-name

3.Open a Pull Request on GitHub:

From feature/your-feature-name → dev

4.After testing, create PR from dev → main

📄 File Structure
lua
Copy
Edit
devops-git-project/
├── README.md
├── .gitignore
├── docs/
│   └── task-log.md
🚫 .gitignore
Includes commonly ignored files:

gitignore
Copy
Edit
*.log
*.tmp
.env
.idea/
node_modules/
target/
🔖 Tags
Release tags are used for versioning.

Example:

bash
Copy
Edit
git tag -a v1.0 -m "Initial release"
git push origin v1.0
