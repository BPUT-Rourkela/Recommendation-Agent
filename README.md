 # Recommendation Agent Prototype

This repository contains a Jupyter notebook exploring the **Amazon product reviews dataset** and building initial recommendation-oriented analyses and models.

## Contents

- **`Amazon Review Dataset EDA and models.ipynb`**: End-to-end exploratory data analysis (EDA) and basic modeling on an Amazon product reviews CSV file. It includes:
  - Loading and inspecting product and review data
  - Data cleaning and type conversions (prices, discounts, ratings, rating counts)
  - Descriptive statistics and visualizations
  - Early experimentation toward building recommendation logic

## Requirements

The notebook primarily uses:

- Python 3.8+  
- `pandas`  
- `numpy`  
- `matplotlib`  
- `seaborn`  
- `scipy`  
  
You can install the core dependencies with:

```bash
pip install pandas numpy matplotlib seaborn scipy
```

## Data

The notebook expects an Amazon reviews CSV file, currently referenced with a local path in one of the cells:

```python
df = pd.read_csv(r"C:\\Users\\rinka\\Desktop\\Recommendation\\amazon.csv\\amazon.csv")
```

To run this notebook on your own machine:

- Place the CSV file anywhere you like.
- Update the path in the notebook to point to your local copy.

## How to Run

1. Create and activate a Python virtual environment (optional but recommended).
2. Install the dependencies listed above.
3. Launch Jupyter:
   ```bash
   jupyter notebook
   ```
4. Open `Amazon Review Dataset EDA and models.ipynb` and run the cells in order.

## Future Improvements

- Generalize data loading so that the CSV path is configurable (e.g. via a relative `data/` folder or environment variables).
- Add modular Python scripts for data preprocessing and model training.
- Introduce more advanced recommendation algorithms and evaluation metrics.

