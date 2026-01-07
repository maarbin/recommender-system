# recommender-system

A recommendation system project using the MovieLens dataset.

## Prerequisites

- Python 3.12+
- [UV](https://docs.astral.sh/uv/) package manager

### Installing UV

**macOS / Linux:**

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

**Windows (PowerShell):**

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

**Homebrew (macOS/Linux):**

```bash
brew install uv
```

## Setup

1. Clone the repository:

   ```bash
   git clone git@github.com:matadcze/recommender-system.git
   cd recommender-system
   ```

2. Install dependencies:
   ```bash
   uv sync
   ```

## Running Notebooks

Start JupyterLab:

```bash
uv run jupyter lab
```

This opens JupyterLab in your browser. Navigate to the `notebooks/` directory and open any notebook.

### Available Notebooks

- `notebooks/start.ipynb` - Initial data exploration with MovieLens ratings data
