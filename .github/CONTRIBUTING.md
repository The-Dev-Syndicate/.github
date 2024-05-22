# Contributing to Projects

Thank you for considering contributing to our projects! We're excited to have you join our community and help build amazing projects with us! This guide will help you get started and ensure that your contributions are valuable and integrated smoothly.

**We welcome contributions from everyone, especially those who are new to open source! This is a fun community for all, and we encourage newcomers to make PRs and help out where they see fit.** 
_Don't worry if your code doesn't make it in on the first try; you will still receive valuable feedback and have the opportunity to grow!_

## How to Contribute

### Reporting Issues
If you find a bug or have a feature request, please report it by creating a new issue in the respective project repository. 
When creating an issue, please provide as much detail as possible to help us understand and address it quickly.

### Forking a Repository
1. Fork the repository to your own GitHub account.
2. Clone the forked repository to your local machine:
    ```sh
    git clone https://github.com/{your-username}/{project}.git
    cd {project}
    ```
3. Set up the upstream remote:
    ```sh
    git remote add upstream https://github.com/Development-Corps/{project}.git
    ```

### Creating a Branch

_**Please note that below 'FF' is representative of our project Feed Fusion. We use 2-3 letter abbreviations for our projects to tie commits/issues to so we can easily identify the related project. For example, if we were working on a project "Super Cool Project," the branch name would be "feature/SCP-{issue_number}"** (this is subject to change in the future!)_

Before starting work on a new feature or bug fix, create a new branch from the `main` branch:

1. Ensure you are on the `main` branch:
    ```sh
    git checkout main
    ```
2. Pull the latest changes:
    ```sh
    git pull upstream main
    ```
3. Create a new branch for your work (using FeedFusion for our example):
    ```sh
    git checkout -b {issue_type}/FF-{issue_number}
    ```
    For example, if you are working on feature issue number 5, you would name your branch:
    ```sh
    git checkout -b feature/FF-5
    ```

### Making Changes
1. Make your changes in the new branch.
2. Commit your changes with a clear and concise commit message (_using FeedFusion for our example):
    ```sh
    git add .
    git commit -m "[FF-{issue_number}] - Add description of the changes made"
    ```
    _Please ensure you tie commits back to an issue with the format `[FF-{issue_number}] - message`. This helps us in case we ever need to do any kind of rollback_.

### Pushing Changes
1. Push your changes to your forked repository:
    ```sh
    git push remote {branch_name}
    ```

### Submitting a Pull Request
1. Go to the original repository on GitHub and create a pull request from your fork.
2. View the [Pull Request Requirements](#pull-request-requirements)
3. Ensure all checks and tests pass before submitting your pull request.

### Pull Request Requirements
_(I know this has been said BUT: using FeedFusion as our example for the 'FF')_

- Please title your PR's using the convention: `[FF-{issue_number}] - {Short Title}`.
  - This helps us tie very quickly back to the issue that is being addresed!
- All pull requests (PRs) must link to the issue they are closing using the keywords "closes #{issue_number}" (_feel free to use any other GitHub-supported keyword; this is just our favoirte_).
  - For example:  
    ```md
    Description and details
    ...
    Merging this PR closes #5
    ```

### Branch Naming Convention

_(Last time I swear: using FeedFusion as our example for the 'FF')_

All branches should have a target issue attached and be named using the following format:

```markdown
{issue_type}/FF-{issue_number}
```

For example, a feature branch for issue number 5 would be: feature/FF-5


### Code Review and Approval
- All PRs should be reviewed by at least one other core developer.
- Ensure the code follows the project's coding standards and guidelines.
- Test the changes locally to confirm they work as expected.

## General Contribution Guidelines

- Be Respectful and Considerate: We welcome contributions from everyone, so please be respectful and considerate in all interactions.
- Write Clear and Concise Code: Ensure your code is easy to read and understand.
- Comment Your Code: Provide comments where necessary to explain your logic and decisions.
- **Keep Changes Small and Focused**: Large changes are harder to review and merge. Try to keep your changes small and focused on a single issue or feature.
- Update Documentation: If your changes affect the documentation, please update it accordingly.

Thank you for contributing to our Projects and Community! Together, we can create amazing tools for everyone to use.