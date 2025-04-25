# 🧠 auto-contrib-bot

Automated GitHub workflow that mimics daily human activity by committing updates, creating issues, and opening pull requests—like a diligent little contribution robot 🤖.

---

## 📌 Features

- ✅ Auto commit once per day (`daily-log.txt` updated)
- ✅ Auto create daily issue
- ✅ Auto open pull request with latest changes
- ✅ Triggered by schedule (`cron`) or manually (`workflow_dispatch`)
- ✅ Safe commit only if changes exist (prevents empty commit error)
- ✅ Easy to customize and extend

---

## 🚀 Usage

This repo is powered by GitHub Actions located in `.github/workflows/auto-actions.yml`.  
You don't need to run anything manually—it's fully automated!

If you want to manually trigger the workflow, go to the **Actions tab** and run it via **"Run workflow"**.

---

## 🛠️ Badge

![Auto Bot Status](https://github.com/YunggiAlyana/auto-contrib-bot/actions/workflows/auto-actions.yml/badge.svg)

---

## 📅 Feature Log

| Date       | Feature/Update                    |
|------------|-----------------------------------|
| 2025-04-25 | Initial release with daily commit |
| 2025-04-25 | Added auto issue and PR creation  |
| 2025-04-25 | Error handling improved            |
| –          | More updates coming soon...       |

---

## 💡 Motivation

This project is inspired by the idea of keeping a GitHub graph active and maintaining momentum in open source contributions—even during busy times.

---

## 🧑‍💻 Made with ❤️ by [@YunggiAlyana](https://github.com/YunggiAlyana)
