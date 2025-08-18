# Python Skeleton

A modern Python project skeleton with UV package management and Ruff linting.

## Features

- 🚀 Simple Python project structure
- 📦 UV package management for fast dependency resolution  
- 🔍 Modern linting and formatting with Ruff
- 🔄 GitHub Actions for CI/CD
- 📝 All configuration in pyproject.toml
- 🐍 Python 3.11 focused

## Prerequisites

- Python 3.11 or higher
- [UV](https://github.com/astral-sh/uv) package manager

## Installation

1. Clone the repository:
```bash
git clone https://github.com/kpandit15/python-skeleton.git
cd python-skeleton
```

2. Install UV if you haven't already:
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

3. Run the script:

```bash
# Create virtual environment
uv venv

# Activate virtual environment
source .venv/bin/activate

# Install dependencies
uv pip install -e ".[dev]"

# Install pre-commit hooks
uv run pre-commit install
```

## Usage

Run the main application:
```bash
python main.py
```

### Code Quality

```bash
# Format code
uv run ruff format src

# Lint code  
uv run ruff check src

# Fix linting issues automatically
uv run ruff check --fix src

# Run pre-commit hooks on all files
uv run pre-commit run --all-files
```

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.