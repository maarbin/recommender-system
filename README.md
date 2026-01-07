# recommender-system

A recommendation system project using the MovieLens dataset.

## Prerequisites

- Python 3.12+
- [UV](https://docs.astral.sh/uv/) package manager

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
