# Jupyter Data Science Environment

A Python Jupyter environment with common data science packages for data analysis, visualization, and machine learning.

## Packages Included

- **Jupyter**: Notebook and Lab interfaces
- **NumPy**: Numerical computing
- **Pandas**: Data manipulation and analysis
- **Matplotlib**: Data visualization
- **Seaborn**: Statistical data visualization
- **Scikit-learn**: Machine learning
- **Plotly**: Interactive visualizations
- **SciPy**: Scientific computing
- **Statsmodels**: Statistical modeling

## Setup Instructions

### Option 1: Using venv (Recommended)

```bash
# Create a virtual environment
python -m venv jupyter_env

# Activate the environment
# On Windows:
jupyter_env\Scripts\activate
# On macOS/Linux:
source jupyter_env/bin/activate

# Install packages
pip install -r requirements.txt

# Start Jupyter
jupyter notebook
```

### Option 2: Using conda

```bash
# Create a conda environment
conda create -n jupyter_env python=3.11

# Activate the environment
conda activate jupyter_env

# Install packages
pip install -r requirements.txt

# Start Jupyter
jupyter notebook
```

## Quick Start

1. Activate your virtual environment
2. Run `jupyter notebook` or `jupyter lab`
3. Create a new notebook and start coding!

## Example Usage

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Create sample data
data = pd.DataFrame({
    'x': np.random.randn(100),
    'y': np.random.randn(100)
})

# Create a scatter plot
plt.figure(figsize=(10, 6))
sns.scatterplot(data=data, x='x', y='y')
plt.title('Sample Scatter Plot')
plt.show()
```

## Project Structure

```
AI-notebooks/
├── requirements.txt    # Package dependencies
├── README.md          # This file
├── notebooks/         # Jupyter notebooks directory
└── data/             # Data files directory
```

## Deactivating the Environment

```bash
# On Windows:
deactivate
# On macOS/Linux:
deactivate
```
