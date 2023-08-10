# Git Workflow Cheat Sheet

## Fresh Application: Create a new develop branch from main

```bash
git checkout main
git pull origin main
git checkout -b develop
git push origin develop
```

# When Develop and Main Branch already exists:

## Create and Work on Feature Branch

```bash
# Create a new feature branch off develop
git checkout develop
git pull origin develop
git checkout -b feature/<branch_name>

# Work on your changes, make commits
git add .
git commit -m "Your commit message"
```

## Push Feature Branch to Remote

```bash
git push origin feature/<branch_name>

```

## Create Pull Request (PR) on GitHub

1. Go to your repository on GitHub.
2. Click on the "Pull Requests" tab.
3. Click the "New Pull Request" button.
4. Set `base` to `develop` and `compare` to your feature branch (`feature/<branch_name>`).
5. Add a title and description for your pull request.
6. Create the pull request.

## Code Review and Approval

- Invite team members to review your pull request.
- Respond to feedback and make necessary changes.
- Team members approve the pull request when satisfied.

## Merge Pull Request on GitHub

1. Once approved, click the "Merge Pull Request" button on GitHub.
2. Choose "Squash and Merge" or "Rebase and Merge" if desired.
3. Confirm the merge.
