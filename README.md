# Shopify App Demand Analysis

#### This repository provides an end-to-end pipeline for analyzing and ranking mobile app categories by demand using unsupervised machine learning. You will compute demand proxies (reviews, ratings, sentiment), perform PCA and clustering, and explore category prevalence within clusters.

## 📦 Requirements

- Python 3.10 or 3.11

- Virtual environment (venv or conda)

#### Core libraries:

- pandas

- numpy

- sqlalchemy

- pymysql

- scikit-learn

- vaderSentiment

- matplotlib

- python-dotenv (optional, for loading .env)

Install via:

``pip install -r requirements.txt``


## 🔧 Setup

1. Clone this repository:



```bash
git clone https://github.com/dot-elements/App-Demand-Predictor-Shopify.git
```



2. **Create** and **activate** your virtual environment(with conda):
```bash
conda create --name app-demand python=3.10
conda activate app-demand
```
3. **Install dependencies:**

``pip install -r requirements.txt``


4. **Database credentials:**
- Create a `.env` file in the project root with:
```dotenv
DB_USER=your_username
DB_PASS=your_password
DB_HOST=hostname_or_ip
DB_PORT=3306
DB_NAME=shopify2024
```

- Set these environment variables manually according to your database.

## 📈 Startup and Results
- After setting up the environment and installing dependencies, you can run the Jupyter notebook to execute the analysis.
- Make sure your environment is activated and the database connection is established.
- Run the following command in your terminal to start Jupyter Notebook:
```bash
jupyter notebook
```
- Open the notebook file `predictor.ipynb` and run the cells sequentially.
- In the **Download Data** section, you can retrieve the app and category results per cluster. Results are saved in the `data` folder as xlsx files.