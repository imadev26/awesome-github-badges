# 🏆 Awesome GitHub Profile Badges

A complete guide to unlock all GitHub Profile Achievement Badges!

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Stars](https://img.shields.io/github/stars/imadev26/awesome-github-badges?style=social)](https://github.com/imadev26/awesome-github-badges)

## 📋 Table of Contents

- [Available Badges](#-available-badges)
- [How to Get Each Badge](#-how-to-get-each-badge)
- [Badge Tiers](#-badge-tiers)
- [Quick Commands](#-quick-commands)
- [Contributing](#-contributing)

---

## 🎖️ Available Badges

| Badge | Name | How to Unlock |
|:-----:|:-----|:--------------|
| 🦈 | **Pull Shark** | Have pull requests merged |
| ⚡ | **Quickdraw** | Close an issue/PR within 5 minutes |
| 🤠 | **YOLO** | Merge a PR without code review |
| 👥 | **Pair Extraordinaire** | Co-author commits in merged PRs |
| 🧠 | **Galaxy Brain** | Have answers accepted in Discussions |
| 🌟 | **Starstruck** | Have a repository with many stars |
| 💖 | **Public Sponsor** | Sponsor an open source developer |
| 🥶 | **Arctic Code Vault** | Contributed to 2020 Archive Program |
| 🚀 | **Mars 2020** | Contributed to Mars Helicopter code |

---

## 🎯 How to Get Each Badge

### 🦈 Pull Shark

> Difficulty: ⭐⭐

```bash
# Create a branch, make changes, and open a PR
git checkout -b feature-branch
echo "New feature" >> README.md
git add . && git commit -m "Add feature"
git push -u origin feature-branch
gh pr create --title "My Feature" --body "Description"
gh pr merge --merge
```

**Tiers:**
- 🥉 Bronze: 2 PRs merged
- 🥈 Silver: 16 PRs merged  
- 🥇 Gold: 128 PRs merged
- 💎 Diamond: 1024 PRs merged

---

### ⚡ Quickdraw

> Difficulty: ⭐

```bash
# Open and close an issue within 5 minutes
gh issue create --title "Quick test" --body "Testing"
gh issue close 1
```

---

### 🤠 YOLO

> Difficulty: ⭐⭐

```bash
# Enable branch protection, then merge as admin
gh api repos/{owner}/{repo}/branches/main/protection -X PUT \
  --input - <<< '{"required_pull_request_reviews":{"required_approving_review_count":1},"enforce_admins":false,"required_status_checks":null,"restrictions":null}'

# Create and merge PR without review
gh pr create --title "YOLO" --body "Living dangerously"
gh pr merge --admin --merge
```

---

### 👥 Pair Extraordinaire

> Difficulty: ⭐⭐

```bash
# Add co-author to your commit
git commit -m "Collaborative work

Co-authored-by: username <username@users.noreply.github.com>"
```

**Tiers:**
- 🥉 Bronze: 1 co-authored commit
- 🥈 Silver: 10 co-authored commits
- 🥇 Gold: 24 co-authored commits
- 💎 Diamond: 48 co-authored commits

---

### 🧠 Galaxy Brain

> Difficulty: ⭐⭐⭐

1. Find repositories with GitHub Discussions enabled
2. Answer questions helpfully
3. Wait for the question author to mark your answer as "Accepted"

**Popular repos with Discussions:**
- [Next.js](https://github.com/vercel/next.js/discussions)
- [React](https://github.com/facebook/react/discussions)
- [Tailwind CSS](https://github.com/tailwindlabs/tailwindcss/discussions)

---

### 🌟 Starstruck

> Difficulty: ⭐⭐⭐⭐

Create a popular repository! Ideas:
- Awesome lists (`awesome-xxx`)
- Useful CLI tools
- Cheat sheets
- Project templates

**Tiers:**
- 🥉 Bronze: 16 stars
- 🥈 Silver: 128 stars
- 🥇 Gold: 512 stars
- 💎 Diamond: 4096 stars

---

### 💖 Public Sponsor

> Difficulty: ⭐

1. Go to [GitHub Sponsors](https://github.com/sponsors)
2. Find a developer to support
3. Sponsor them (even $1/month counts!)

---

## 📊 Badge Tiers

| Badge | Bronze | Silver | Gold | Diamond |
|:------|:------:|:------:|:----:|:-------:|
| Pull Shark | 2 | 16 | 128 | 1024 |
| Pair Extraordinaire | 1 | 10 | 24 | 48 |
| Galaxy Brain | 2 | 8 | 16 | 32 |
| Starstruck | 16 | 128 | 512 | 4096 |

---

## 🚀 Quick Commands

```bash
# Install GitHub CLI
winget install GitHub.cli

# Login
gh auth login

# Create repo
gh repo create my-repo --public --clone

# Create and merge PR (Pull Shark)
git checkout -b feature
echo "content" >> file.txt
git add . && git commit -m "Add feature"
git push -u origin feature
gh pr create -t "Title" -b "Body"
gh pr merge --merge --delete-branch

# Quick issue (Quickdraw)
gh issue create -t "Test" -b "Test"
gh issue close 1
```

---

## 🤝 Contributing

Feel free to:
- ⭐ Star this repo if you found it helpful!
- 🐛 Open issues for questions
- 🔀 Submit PRs to improve this guide

---

## 📜 License

MIT License - Feel free to use and share!

---

Made with ❤️ by [@imadev26](https://github.com/imadev26)
