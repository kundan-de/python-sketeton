# Contributing to Python Skeleton

First off, thank you for considering contributing to Python Skeleton! It's people like you that make this project great.

### Pull Requests

1. Create your branch from `main`
5. Make sure your code lints

## Development Setup

1. Clone your fork of the repository:
```bash
git clone https://github.com/YOUR_USERNAME/python-skeleton.git
cd python-skeleton
```

2. Install UV if you haven't already:
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

3. Create a virtual environment and install dependencies:
```bash
uv venv
source .venv/bin/activate
uv pip install -e ".[dev]"

# Install pre-commit hooks
uv run pre-commit install
```

## Development Workflow

### Before Making Changes

1. Create a new branch for your feature/fix:
```bash
git checkout -b feature/your-feature-name
```

### Making Changes

1. Write your code following the project's style guidelines
2. Update documentation if necessary
3. Run the linting tools:
```bash
uv run ruff check src
uv run ruff format src
```

### Before Committing

1. Run all quality checks:
```bash
uv run ruff check src && uv run ruff format --check src
```

Or run pre-commit hooks (which will also run automatically on commit):
```bash
uv run pre-commit run --all-files
```

2. Commit your changes (pre-commit hooks will run automatically):
```bash
git add .
git commit -m "Add your descriptive commit message"
```

### Submitting Changes

1. Push your branch to your fork:
```bash
git push origin feature/your-feature-name
```

2. Create a pull request from your fork to the main repository

## Style Guidelines

### Python Code Style

- Use Ruff for formatting and linting
- Write docstrings for all public functions and classes
- Keep lines under 105 characters

### Git Commit Messages

- Use the present tense ("Add feature" not "Added feature")
- Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
- Limit the first line to 72 characters or less
- Reference issues and pull requests liberally after the first line

## Code Review Process

1. All submissions require review before merging
2. Reviewers will look for:
   - Code quality and style
   - Documentation updates
   - Performance implications
   - Security considerations
