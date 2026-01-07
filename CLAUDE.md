# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A recommendation system project in early development stage. Currently focused on data exploration via Jupyter notebooks with planned API and web components.

## Tech Stack

- **Python**: 3.12
- **Package Manager**: UV (uses `uv.lock` for reproducibility)
- **Core Libraries**: pandas, numpy, scikit-learn, matplotlib, seaborn
- **Interactive Development**: Jupyter/JupyterLab

## Commands

```bash
# Install dependencies
uv sync

# Run main entry point
uv run python main.py

# Start Jupyter Lab
uv run jupyter lab

# Run a specific notebook
uv run jupyter execute notebooks/start.ipynb
```

## Project Structure

```
recommender-system/
├── api/           # API layer (planned)
├── data/          # Data storage (raw/processed)
├── notebooks/     # Jupyter notebooks for exploration
├── web/           # Web interface (planned)
└── main.py        # Entry point
```

## Data

The project uses MovieLens dataset. Raw data is stored at `data/raw/movielens/rating.csv`.
