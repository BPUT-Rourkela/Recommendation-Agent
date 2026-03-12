 # Recommendation and Sentiment Analysis Prototype

This repository contains tools and notebooks for exploring the **Amazon product reviews dataset**, building recommendation systems, and performing sentiment analysis.

## Project Structure

- **`Sentiment_Analysis.ipynb`**: Comprehensive sentiment analysis workflow. It includes:
  - Text preprocessing (cleaning, tokenization, stemming).
  - Exploratory Data Analysis (EDA) of review sentiments.
  - Multi-model evaluation (Logistic Regression, Random Forest, XGBoost, LightGBM, etc.).
  - Saving trained models to `Sentiment_Models/`.
- **`prototype/Amazon Review Dataset EDA and models.ipynb`**: Initial EDA and recommendation system experimentation.
- **`Sentiment_Models/`**: Directory containing pre-trained sentiment classification models (Pickle format).
- **Pre-trained Recommender Files**:
  - `knn_recommender_model.pkl`: Recommender system based on K-Nearest Neighbors.
  - `products_dataframe.pkl`, `tfidf_matrix.pkl`, `tfidf_vectorizer.pkl`: Data and features for the recommendation engine.

## Requirements

The project requires Python 3.8+ and the following libraries:

```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn nltk xgboost lightgbm vaderSentiment imbalanced-learn watermark plotly datasets
```

## Data

The notebooks expect an Amazon reviews CSV file (`amazon.csv`). Currently, the notebooks reference a local path:

```python
df = pd.read_csv(r"C:\\Users\\rinka\\Desktop\\Recommendation\\amazon.csv\\amazon.csv")
```

To run these notebooks:
- Place the `amazon.csv` file in the expected path (or update the path in the notebook).
- Ensure all dependencies are installed.

## How to Run

1. Create and activate a Python virtual environment.
2. Install the core dependencies.
3. Launch Jupyter:
   ```bash
   jupyter notebook
   ```
4. Open either `Sentiment_Analysis.ipynb` or the notebook in `prototype/` to begin analysis.

## Future Improvements

- Modularize Python scripts for cleaner integration.
- Deploy a web-based interface for real-time recommendations and sentiment scoring.
- Incorporate Deep Learning models (e.g., BERT) for enhanced sentiment accuracy.

