# 📚 Scopus RecSys - Comprehensive Recommender System Analysis

This repository contains three main components for exploring, analyzing, and documenting recommender systems in academic literature from Scopus:

1. **Scopus RecSys Explorer**: An interactive Streamlit application for visualizing and exploring recommender systems algorithms and their applications.
2. **Scopus RecSys Job**: A system for classifying, analyzing, and finding similarities between research papers, with a focus on recommender systems.
3. **Scopus RecSys Documentation**: A repository to generate a detailed article about the Scopus RecSys workflow.

## 🌟 Features

### Scopus RecSys Explorer
- **Statistics Dashboard**: View key metrics about algorithms and applications in the dataset.
- **Interactive Heatmap**: Explore relationships between algorithms and applications with adjustable occurrence thresholds.
- **Algorithm Explorer**: Discover applications associated with specific algorithms through interactive word clouds.
- **Application Explorer**: Find algorithms commonly used in specific application domains.

### Scopus RecSys Job
- **Paper Classification**: Automatically classifies research papers based on their abstracts using Large Language Models.
- **Algorithm Similarity**: Calculates similarities between different algorithms mentioned in papers.
- **Application Similarity**: Identifies similar applications across different papers.
- **Algorithm-Application Linking**: Creates connections between algorithms and their applications.
- **Database Management**: Efficient SQLite database handling for storing and retrieving paper information.

### Scopus RecSys Documentation
- **Workflow Article**: Generates a detailed article about the Scopus RecSys workflow, providing insights into the system's architecture and processes.

## 🚀 Getting Started

### Prerequisites

- Python 3.6+
- pip (Python package installer)
- Docker (for Scopus RecSys Job)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/scopus-recsys.git
   cd scopus-recsys
   ```

2. Install the required dependencies for the Explorer:
   ```bash
   cd scopus-recsys-app
   pip install -r requirements.txt
   ```

3. Set up the environment for the Job:
   ```bash
   cd ../scopus-recsys-job
   # Set up environment variables in `.env`
   uv venv
   source .venv/bin/activate
   uv pip install -r requirements.txt
   ```

### Running the Applications

#### Scopus RecSys Explorer
Run the Streamlit application:
```bash
cd scopus-recsys-app
streamlit run streamlit_app.py
```
The application will open in your default web browser at `http://localhost:8501`.

#### Scopus RecSys Job
Run the system using Docker:
```bash
cd scopus-recsys-job
docker-compose up -d
```

## 📊 Data

The applications use a DuckDB database (`data/db.duckdb`) and SQLite for storing and processing data related to algorithms, applications, and research papers.

## 🛠️ Tech Stack

- **Streamlit**: Web application framework
- **DuckDB & SQLite**: Database engines
- **Pandas & Numpy**: Data manipulation
- **Plotly & WordCloud**: Interactive visualizations
- **Typer & Loguru**: CLI and logging for the Job system

## 📝 License

This project is licensed under the Apache License - see the LICENSE file for details.

