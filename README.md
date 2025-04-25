# 🤖 auto-contrib-bot

An automated GitHub workflow that simulates daily activity by creating commits, issues, and pull requests—boosting your contribution graph with zero manual effort!

![GitHub Actions Status](https://github.com/YunggiAlyana/auto-contrib-bot/actions/workflows/auto-actions.yml/badge.svg)

## ✨ Features

- ✅ **Automated Daily Commits** - Maintains your GitHub activity streak
- ✅ **Daily Issue Creation** - Demonstrates engagement on your repository
- ✅ **Automated Pull Requests** - Shows code review and collaboration activity
- ✅ **Fully Configurable** - Customize frequency, content, and behavior
- ✅ **Zero Manual Effort** - Set it up once and let it run

## 🚀 How It Works

This bot runs on GitHub Actions and performs these tasks on a schedule:

1. **Updates a daily log file** with timestamps and run information
2. **Creates an issue** with the current date and run details
3. **Opens a pull request** with the latest changes to the daily log

All activities are performed by the GitHub Actions bot with proper authentication using your provided token.

## 📋 Setup Instructions

### 1. Fork or Clone This Repository

Start by forking this repository to your GitHub account.

### 2. Set Up the Required Secret

1. Go to your repository's **Settings** tab
2. Navigate to **Secrets and variables** > **Actions**
3. Create a new repository secret:
   - Name: `MY_GITHUB_TOKEN`
   - Value: Your GitHub Personal Access Token with `repo` permissions

### 3. Enable GitHub Actions

1. Go to the **Actions** tab in your repository
2. Enable workflows if they aren't already enabled
3. The workflow is set to run automatically every day at 12:00 UTC

### 4. Customize (Optional)

Feel free to modify the workflow file at `.github/workflows/auto-actions.yml` to:
- Change the schedule using cron syntax
- Modify the content added to the daily log
- Customize issue and PR templates

## 📊 Example Output

### Daily Log
```
Updated on: 2025-04-25 12:00:00 UTC
Current run number: 1
Updated on: 2025-04-26 12:00:00 UTC
Current run number: 2
```

### Daily Issue
```
# Daily Contribution Report

- Date: 2025-04-25
- Run Number: 1

This issue was automatically created by the auto-contrib-bot.
```

## 🛠️ Troubleshooting

### Common Issues

1. **Workflow failing with permission errors**
   - Make sure your `MY_GITHUB_TOKEN` has the correct permissions
   - Check that workflow permissions are set to "Read and write permissions" in repository settings

2. **Pull request creation failing**
   - This usually happens if there are no changes between branches
   - The workflow is designed to avoid this by adding new content daily

## 📅 Future Enhancements

- [ ] Add randomized commit messages
- [ ] Support for multiple file types and templates
- [ ] Statistics dashboard for tracking contributions
- [ ] Customizable activity patterns and frequency

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⭐ Support

If you find this project helpful, please give it a star! And feel free to fork and customize it for your own needs.

## 🧑‍💻 Created by [@YunggiAlyana](https://github.com/YunggiAlyana)

Want to contribute? Pull requests are welcome!
