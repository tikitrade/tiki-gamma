# Contributing to Tiki Gamma

First off, thank you for considering contributing to Tiki Gamma! It's people like you that make the open-source community such a great place to learn, inspire, and create.

We welcome contributions of all kinds, from bug fixes to new features, and especially entirely new related indicators that leverage the levels data.

## How Can I Contribute?

### Reporting Bugs
If you find a bug, please open an issue and include:
- A clear and descriptive title.
- Steps to reproduce the bug.
- Expected behavior vs actual behavior.
- Screenshots if applicable.

### Suggesting Enhancements
If you have an idea for a new feature or an improvement to an existing one, please open an issue and describe:
- The problem it solves.
- Your proposed solution.
- Any alternatives you've considered.

### Pull Requests
1. Fork the repository and create your branch from `main`.
2. Ensure your code follows the existing style conventions.
3. Update documentation if necessary (e.g., README.md, docs/tradingview-description.md, Pine Script header comments).
4. Make sure your commit messages follow our commit structure guidelines below.
5. Open a Pull Request! Please provide a clear description of what your PR does and include screenshots of visual changes on TradingView.

## Commit Guidelines

We use [Conventional Commits](https://www.conventionalcommits.org/) and commitlint to enforce consistent, readable commit messages. 

Your commit message should be structured as follows:
```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

### Types
Must be one of the following:
- **feat**: A new feature
- **fix**: A bug fix
- **docs**: Documentation only changes
- **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
- **refactor**: A code change that neither fixes a bug nor adds a feature
- **perf**: A code change that improves performance
- **test**: Adding missing tests or correcting existing tests
- **build**: Changes that affect the build system or external dependencies
- **ci**: Changes to our CI configuration files and scripts
- **chore**: Other changes that don't modify src or test files
- **revert**: Reverts a previous commit

### Example
```
feat(indicator): add toggles for max pain expansion
```

## Creating Related Indicators
We'd love to see what you can build using the levels data! If you create a new indicator that you think would be valuable to the community:
1. Create a new folder for your indicator within this repository, or link to your external repository in an issue for us to highlight in our README.
2. Provide clear documentation on how it works, what it visualizes, and how to use it.
3. Submit a PR for us to review and potentially feature your work!

## Code of Conduct
Please note that this project is released with a Contributor Code of Conduct. By participating in this project you agree to abide by its terms. Let's keep the community welcoming and respectful!
