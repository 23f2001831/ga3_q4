# GA3 Q4: Daily DevSync Commit Automation

![Daily DevSync Commit](https://github.com/23f2001831/ga3_q4/actions/workflows/daily-commit.yml/badge.svg)

This repository contains a scheduled GitHub Action that runs daily and commits to the repository automatically.

## Workflow Details

- **Schedule**: Runs at 12:30 UTC every day (`30 12 * * *`)
- **Email**: 23f2001831@ds.study.iitm.ac.in
- **Purpose**: Track daily activity with automated commits

## Files

- `.github/workflows/daily-commit.yml` - The GitHub Actions workflow configuration
- `activity_log.txt` - Log file tracking daily activity

## Manual Testing

To test the workflow immediately without waiting 24 hours:

1. Go to your GitHub repository
2. Click on the **Actions** tab
3. Select **Daily DevSync Commit** from the left menu
4. Click **Run workflow** → **Run workflow**
5. Wait for the workflow to complete (usually 10-30 seconds)
6. Verify that a new commit was created with "Automated daily activity log update"

## How It Works

Each day at 12:30 UTC, the workflow:
1. Checks out the repository
2. Appends a timestamp to `activity_log.txt`
3. Commits the changes
4. Pushes back to the repository

This provides activity tracking, automated documentation, backup, and compliance logging.
