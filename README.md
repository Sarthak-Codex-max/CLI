---

# 🖥 GitHub CLI (gh) Commands Reference

This repository also includes practice using **GitHub CLI (`gh`)**, which allows managing GitHub directly from the terminal.

---

## 🔐 Authentication Commands

Login to GitHub:

```bash
gh auth login
```

Check login status:

```bash
gh auth status
```

Logout:

```bash
gh auth logout
```

Refresh permissions (example: delete repo permission):

```bash
gh auth refresh -h github.com -s delete_repo
```

---

## 📦 Repository Management

Create a new repository:

```bash
gh repo create repo-name --public
```

Create a repo from current folder and push immediately:

```bash
gh repo create repo-name --source=. --remote=origin --push
```

List your repositories:

```bash
gh repo list
```

View repository in browser:

```bash
gh repo view --web
```

Delete repository (requires delete_repo scope):

```bash
gh repo delete username/repository-name
```

---

## 🐞 Issue Management

Create a new issue:

```bash
gh issue create
```

List issues:

```bash
gh issue list
```

View a specific issue:

```bash
gh issue view <issue-number>
```

---

## 🔀 Pull Request (PR) Workflow

Create a pull request:

```bash
gh pr create
```

List pull requests:

```bash
gh pr list
```

View a pull request:

```bash
gh pr view
```

Merge a pull request:

```bash
gh pr merge
```

Open PR in browser:

```bash
gh pr view --web
```

---

# 🚀 Example Professional Workflow Using gh

1. Create repository:
```bash
gh repo create project --public --source=. --remote=origin --push
```

2. Create a new feature branch:
```bash
git switch -c feature-branch
```

3. Push branch:
```bash
git push -u origin feature-branch
```

4. Create pull request:
```bash
gh pr create
```

5. Merge pull request:
```bash
gh pr merge
```

---

# 🧠 Important Concepts

- `gh` interacts with GitHub using API
- Authentication is token-based (stored securely)
- SSH is used for Git operations
- CLI enables full workflow without browser

---

# 🎯 Key gh Commands to Remember

```
gh auth login
gh repo create
gh repo delete
gh issue create
gh pr create
gh pr merge
```

These are sufficient for most real-world development workflows.

---

# 📌 Summary

Using GitHub CLI allows:

- Managing repositories from terminal
- Creating and managing issues
- Creating and merging pull requests
- Automating workflows
- Operating like a professional developer

This enhances productivity and reduces dependency on the web interface.
