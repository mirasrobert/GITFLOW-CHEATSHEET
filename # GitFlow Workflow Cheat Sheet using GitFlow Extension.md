# GitFlow Workflow Cheat Sheet using GitFlow Extension

## Fresh Application: Initialize GitFlow

1. Initialize GitFlow in your repository:
   ```bash
   git flow init
   ```

# When Develop and Main Branch already exists:

## Create and Work on Feature Branch

```bash
# Create a new feature branch off develop
git flow feature start <branch_name>

# Work on your changes, make commits
git add .
git commit -m "Your commit message"
# (you can directly finish without pushing, but push is recommended)
git push origin feature/<branch_name>
```

## Merging WithOut Pull Request:

## Merge Feature Branch to Develop and Delete Feature Branch:

```bash
git flow feature finish <branch_name>
```

## Merging With Pull Request:

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
