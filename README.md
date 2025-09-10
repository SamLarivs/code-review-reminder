# Daily Code Review Reminders

This repository contains a GitHub Actions workflow that automatically creates daily code review reminder issues.

## Setup

1. **Create Labels**: Go to Issues → Labels in this repository and create:
   - `daily` label (suggested color: #0075ca)
   - `review` label (suggested color: #d73a4a)

2. **Update Username**: The workflow is configured to assign issues to: MY_USERNAME
   - If this needs to be changed, edit `.github/workflows/daily-issue.yml` line 95

3. **Test**: You can manually trigger the workflow from Actions → Daily Code Review Reminder → Run workflow

## How It Works

- Creates one issue per weekday (Monday-Friday)
- Issues appear at random times between 9:00 AM and 11:59 PM ET
- Automatically handles daylight saving time
- Prevents duplicate issues for the same day
- Each issue contains a checklist for code review activities

# Code Review Notes

Daily notes from code review activities. Each file corresponds to a completed daily review issue.

## Structure

Notes are organized by year and month:
- `YYYY/MM-monthname/YYYY-MM-DD.md`

## Template

Each daily note follows the template in `template.md`.

## Quick Links

- [Current Month](./2025/01-january/)
- [Template](./template.md)