# Fake News Detection using Natural Language Processing
**Course:** Machine Learning for Data Analytics  
**Team members:** Karolina B., Amelia B., Agnieszka S., Aleksandra S.

---


## Project Overview
This project aims to develop a robust machine learning system to classify news articles as authentic or misinformation. We utilize advanced NLP techniques, experiment tracking via MLflow, and model interpretability tools like SHAP to ensure transparency in our predictions.

---

## Getting Started

### 1. Environment Setup
To ensure reproducibility, all team members must use the same Python 3.12 environment.

```bash
# Clone the repository
git clone https://github.com/AmeliaBieda/fake-news-detection-ML.git
cd fake-news-detection-ML

# Create and activate a virtual environment
python -m venv venv
# Windows:
.\venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

### 2. Data Management
The `data/` directory is excluded from version control to prevent large file uploads. Team members must manually set up the following local structure:

Create` data/raw/` and `data/processed/` folders.

Download the dataset [https://www.cs.ucsb.edu/~william/data/liar_dataset.zip](https://www.cs.ucsb.edu/~william/data/liar_dataset.zip) and place raw files into `data/raw/`.

### 3. Experiment Tracking
We use MLflow for experiment tracking. To launch the tracking UI locally, run:

``` Bash
mlflow ui
```
The dashboard will be available at `http://localhost:5000`.

---

## Git Workflow and Collaboration
We strictly follow a feature-branching strategy to maintain a clean version history.

- **main**: Contains stable, presentation-ready code only.
- **develop**: Integration branch for merging and testing features.
- **feature/[task-name]**: Individual branches for specific tasks (e.g., `feature/eda`).

**Contribution Rules**:
- Do not commit directly to the `main` branch.
- Submit a Pull Request to merge features into `develop` for team review.
- Use descriptive commit messages.

---

## Repository Structure

- `data/`: Local storage for `raw/` and `processed/` datasets (Git ignored).
- `notebooks/`: Numbered Jupyter Notebooks for EDA, modeling, and analysis (suggested: `01_eda.ipynb`, `02_feature_engineering.ipynb`, `03_modeling.ipynb`, `04_interpretability.ipynb`, `05_final_report.ipynb`).
- `src/`: Reusable Python source code and utility scripts (like `data_loader.py`, `features.py`, `models.py`).
- `reports/`: Presentation materials and exported visualizations.
- `mlruns/`: Local MLflow experiment logs (Git ignored).

---