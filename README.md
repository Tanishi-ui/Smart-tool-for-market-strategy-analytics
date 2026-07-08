# Apple vs. Samsung Product Analysis & Predictive Modeling

An analytical study and machine learning workflow exploring dataset characteristics, price-to-rating distributions, and consumer trends for Apple and Samsung products. This repository includes data extraction, preprocessing, visualization, and a trained predictive model saved for deployment.

---

## 📌 Project Overview
This project performs an exploratory and predictive analysis of Apple and Samsung consumer products. By examining metrics such as prices, star ratings, and review counts, we uncover distinct patterns in brand positioning, customer satisfaction, and pricing strategies. 

Additionally, a machine learning model is trained on the data to predict target metrics, with the final model serialized as `samsung_model.pkl` for integrated application usage.

---

## 🛠️ Built With
- **Python 3**
- **Jupyter Notebook** (Data exploration and model building)
- **Pandas** & **NumPy** (Data cleaning and preprocessing)
- **Seaborn** & **Matplotlib** (Statistical visualizations)
- **Scikit-Learn** (Machine learning modeling and evaluation)
- **Joblib** (Model serialization)
- **Gdown** (Automated dataset fetching from cloud storage)

---

## 📁 Repository Structure
```text
├── final.ipynb            # Main Jupyter Notebook containing the analysis & training code
├── README.md              # Project documentation and guide
├── .gitignore             # Specifies intentionally untracked files to ignore
└── requirements.txt       # Dependencies required to execute the environment
```

---

## 🚀 Getting Started

### 1. Prerequisites
Ensure you have Python installed. It is highly recommended to use a virtual environment to manage dependencies:

```bash
# Create a virtual environment
python -m venv venv

# Activate virtual environment
# On macOS/Linux:
source venv/bin/activate
# On Windows:
venv\Scripts\activate
```

### 2. Install Dependencies
Install all the required Python libraries using the generated `requirements.txt` file:

```bash
pip install -r requirements.txt
```

### 3. Run the Analysis
To run the notebook and download the datasets dynamically:

1. Launch Jupyter Notebook or JupyterLab:
   ```bash
   jupyter notebook
   ```
2. Open `final.ipynb`.
3. Run the cells sequentially. The notebook uses `gdown` to automatically retrieve the datasets (`apple_products.csv` and `samsung.Dataset.csv`) directly from a secure cloud backup, ensuring reproducibility without having to host large static CSV files in this repository.

---

## 📊 Key Findings & Visualizations
- **Pricing Strategy**: Compares distribution scales between high-tier premium Apple devices and Samsung's highly diverse product line spanning budget to flagship tiers.
- **Consumer Ratings**: Analyzes density plots of ratings vs. price points to identify optimal product sweet-spots.
- **Model Serialization**: Generates `samsung_model.pkl` using Scikit-Learn pipelines to allow integration of the trained predictor into production web APIs or lightweight analytical dashboards.

---

## 📄 License
This project is open-source and available under the [MIT License](LICENSE).
