# Contributing to [Loverary]



## Table of Contents
1. [Getting Started](#getting-started)
2. [Branches](#branches)
3. [Commits](#commits)
4. [Pull Requests](#pull-requests)
5. [Code Style](#code-style)
6. [Issue Tracking](#issue-tracking)
7. [Review Process](#review-process)
8. [Communication](#communication)
9. [Additional Notes](#additional-notes)

## Getting Started

1. **Fork the repository** to your own GitHub account.
2. **Clone your fork** to your local machine:
    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    ```
3. **Set up the upstream remote**:
    ```bash
    git remote add upstream https://github.com/original-username/original-repo-name.git
    ```

## Branches

- **main**: This branch contains the stable version of the project. All production-ready code is merged here.
- **development**: This is the branch where all development takes place. Features and fixes should be merged here first.

### Creating a Branch

1. Always create a new branch from the `development` branch:
    ```bash
    git checkout development
    git pull upstream development
    git checkout -b feature/your-feature-name
    ```

## Commits

- Write clear, concise commit messages.
- Use the present tense ("Add feature" not "Added feature").
- Capitalize the first letter of the commit message.
- Limit the first line to 72 characters or less.
- Reference issues and pull requests liberally.

### Commit Message Structure

1. **Type**: feat, fix, docs, style, refactor, test, chore
2. **Scope**: Component or file name (optional)
3. **Subject**: Brief summary of the change
4. **Body**: Detailed explanation (if necessary)

#### Example

```markdown
feat(auth): add login functionality

- Implemented login functionality using OAuth
- Updated user model to include authentication tokens

Resolves #45
```

## Pull Requests

1. **Pull from the `development` branch** before starting your work:
    ```bash
    git pull upstream development
    ```
2. **Push your branch** to your fork:
    ```bash
    git push origin feature/your-feature-name
    ```
3. **Create a pull request** to merge your branch into `development`:
    - Provide a clear title and description.
    - Link any relevant issues.
    - Request reviews from team members.
4. **Ensure your pull request passes all checks** (e.g., CI/CD pipelines, unit tests).

## Code Style

- Follow the coding standards used in the project.
- Run linters and formatters before pushing changes.
- Document your code thoroughly.

### Example

- For Java, use standard Java conventions and ensure your code is formatted using the style guide configured in IntelliJ IDEA.

## Issue Tracking

- Use GitHub Issues to track bugs, feature requests, and improvements.
- Assign labels to categorize issues (e.g., bug, enhancement, documentation).
- Use a template for reporting issues to ensure all necessary information is provided.

### Example Issue Template

```markdown
**Description**

A clear and concise description of what the issue is about.

**Steps to Reproduce**

1. Go to '...'
2. Click on '...'
3. Scroll down to '...'
4. See error

**Expected behavior**

A clear and concise description of what you expected to happen.

**Screenshots**

If applicable, add screenshots to help explain your problem.

**Additional context**

Add any other context about the problem here.
```

## Review Process

1. Pull requests will be reviewed by one team member.
2. Provide constructive feedback and request changes if necessary.
3. Approve the pull request once it meets all requirements and standards.
4. The reviewer merges the pull request into `development`.

## Communication

- Use our telegram group for general questions and support.
- Schedule regular meetings to discuss progress and roadblocks.

## Additional Notes

- Stay up-to-date with the latest changes by regularly pulling from the upstream repository.
- Respect the project's code of conduct.

Let's kick some ass together. 
