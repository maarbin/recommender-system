# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A recommendation system project using the MovieLens dataset. Currently focused on data exploration via Jupyter notebooks with planned API and web components.

## Tech Stack

- **Python**: 3.12
- **Package Manager**: UV (uses `uv.lock` for reproducibility)
- **Core Libraries**: pandas, numpy, scikit-learn, matplotlib, seaborn
- **Infrastructure**: Docker Compose with PostgreSQL 16 and Apache Spark 4.1.0

## Commands

```bash
# Install dependencies
uv sync

# Start infrastructure (PostgreSQL, Spark)
docker-compose up -d

# Stop infrastructure
docker-compose down

# Run main entry point
uv run python main.py

# Start Jupyter Lab
uv run jupyter lab
```

## Infrastructure

- **PostgreSQL**: port 5432, credentials `recommender`/`recommender`, database `recommender`
- **Spark Master**: UI at http://localhost:8080, master port 7077
- **Spark Worker**: 2GB memory, 2 cores

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
