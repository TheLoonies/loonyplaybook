# 🛠️ The LoonyDevs Playbook

> How we write, review, and ship clean code together

![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)
![Protected Branches](https://img.shields.io/badge/main-protected-orange)

---

## 👥 Team Roles

### 🧑‍💻 Core Developers
- Full repo access (Admin or Write)
- Responsible for code reviews, merges, and maintaining repo health

### 🌱 Junior Developers
- Limited to **Write** or **Triage** access per project
- Can open pull requests, but cannot merge to protected branches
- Must request a review from a Core Developer

### 🤝 External Contributors
- Only granted **Read** or **Write** access to specific repos
- PRs require approval from a Core Developer

### 🎨 Designers
- Read or Triage access
- Provide visual/UI feedback
- Participate in PR reviews when needed

---

## 🔁 Branching Strategy

- `main`: Production-ready code only
- `develop`: Ongoing development (optional in larger apps)
- `feature/*`: New features
- `bugfix/*`: Fixes for known issues

> **❌ Never push directly to `main` or `develop`.** Always use a feature or bugfix branch.

---

## ✅ Pull Request Process

1. Create a branch off `develop` or `main`:
   ```
   git checkout -b feature/your-feature-name
   ```

2. Make changes and commit with meaningful messages.

3. Push your branch and open a Pull Request:
   - Include a summary
   - Reference related issues (if any)
   - Request a review from `@Engulfedleader2` or `@ItzYaBoiiJoe`

4. PRs **must be approved** by a Core Developer before merging.

5. Do **not** merge your own PR unless explicitly allowed.

---

## 📑 CODEOWNERS
A `.github/CODEOWNERS` file should exist in every repo to auto-request reviews.

Example:
```
* @Engulfedleader2 @ItzYaBoiiJoe
```

---

## 📋 Pull Request Template
Use the standard PR template to make reviews easier.

```md
### 📋 Summary
What does this PR do?

### ✅ Checklist
- [ ] Code compiles
- [ ] I’ve manually tested this
- [ ] I’ve requested a review from @Engulfedleader2 or @ItzYaBoiiJoe

### 🔍 Notes for Reviewers
(Any important context)
```

Place this file in `.github/PULL_REQUEST_TEMPLATE.md`

---

## 🔐 Security & Access
- All private repos use the **Free Org Plan** — branch protection is process-based
- Team access is scoped **repo-by-repo** (no default access)
- Junior and external contributors only access what they’re assigned

---

## 📦 Repo Template Usage
To start a new project:
1. Duplicate an existing repo or use this guide as a baseline
2. Set up `.github/` directory:
   - `CODEOWNERS`
   - `PULL_REQUEST_TEMPLATE.md`
3. Create `main`, `develop`, and any initial branches

---

## 🧠 Notes
- This guide should be updated as the team grows
- Use GitHub Projects for roadmap planning
- Label issues with `good first issue`, `bug`, `enhancement`, etc.

---

Welcome aboard! 🚀
