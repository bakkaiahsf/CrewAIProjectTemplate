# CrewAI Project Template

This repository provides a robust template for developing your own CrewAI-based framework. It includes a recommended project structure, sample code, configuration schemas, and all the essentials to get started quickly.

## Project Structure Overview

```
crewai/
│   .env.example         # Example environment variables (not tracked by git)
│   .gitignore           # Files and folders to ignore in git
│   LICENSE              # Project license (MIT by default)
│   README.md            # This file
│   requirements.txt     # Python dependencies
│   setup.py             # Packaging and installation script
│
├── docs/                # Project documentation
│   └── getting_started.md
│
├── tests/               # Unit and integration tests
│   └── test_basic.py
│
├── crewai/              # Main package source code
│   ├── __init__.py      # Marks this directory as a Python package
│   ├── main.py          # Example entry point
│   ├── config.py        # Configuration logic
│   ├── agents.py        # Agent class definitions
│   ├── tasks.py         # Task class definitions
│   ├── utils.py         # Utility functions
│   ├── exceptions.py    # Custom exception classes
│   ├── README.md        # Package-level documentation
│   ├── api/             # (Optional) API-related code
│   │   └── __init__.py
│   ├── agent.yaml       # Example agent configuration schema
│   ├── task.yaml        # Example task configuration schema
│   └── crew.yaml        # Example crew configuration schema
│
└── venv/                # Python virtual environment (not tracked by git)
```

## File & Directory Descriptions

- **.env.example**: Template for environment variables. Copy to `.env` and fill in your secrets locally.
- **.gitignore**: Ensures sensitive and unnecessary files (like `venv/`, `__pycache__/`, `.env`) are not tracked by git.
- **LICENSE**: The license for your project (MIT by default, edit as needed).
- **README.md**: Project overview and structure (this file).
- **requirements.txt**: List of Python dependencies for your project.
- **setup.py**: Script for packaging and installing your framework.
- **docs/**: Documentation folder. Start with `getting_started.md` for onboarding.
- **tests/**: Contains unit and integration tests. Start with `test_basic.py`.
- **crewai/**: Main source code for your framework.
  - **__init__.py**: Marks the directory as a Python package.
  - **main.py**: Example entry point for running your framework.
  - **config.py**: Configuration logic and helpers.
  - **agents.py**: Define your agent classes here.
  - **tasks.py**: Define your task classes here.
  - **utils.py**: Utility/helper functions.
  - **exceptions.py**: Custom exception classes for your framework.
  - **README.md**: Documentation specific to the `crewai` package.
  - **api/**: (Optional) Place for API-related code (REST, GraphQL, etc.).
  - **agent.yaml**: Example schema for agent configuration.
  - **task.yaml**: Example schema for task configuration.
  - **crew.yaml**: Example schema for crew configuration.
- **venv/**: Python virtual environment for dependency isolation (not tracked by git).

## Getting Started

1. **Clone the repository**
2. **Create and activate a virtual environment:**
   ```sh
   python -m venv venv
   # On Windows:
   venv\Scripts\activate
   # On macOS/Linux:
   source venv/bin/activate
   ```
3. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```
4. **Start developing your CrewAI framework!**

For more details, see `docs/getting_started.md`. 
