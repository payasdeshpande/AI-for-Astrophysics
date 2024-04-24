### **Evolutionary Stage of Stars**

#### Overview
This Jupyter Notebook is designed to classify stars into their evolutionary stages using data from the Gaia database. It leverages Python libraries such as `astroquery`, `pandas`, `matplotlib`, `seaborn`, `sklearn`, and others to perform data retrieval, preprocessing, visualization, model training, and evaluation.

#### Requirements
- Python 3.x
- Jupyter Notebook
- Libraries: `astroquery`, `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`, `sklearn`, `imblearn`

To install the required Python libraries, run:
```bash
pip install astroquery pandas numpy matplotlib seaborn plotly scikit-learn imblearn
```

#### Detailed Steps

1. **Importing Libraries**
   - The notebook begins by installing and importing necessary Python libraries that facilitate data fetching, manipulation, and visualization.

2. **Data Acquisition**
   - Data is fetched from the Gaia database using the `astroquery.gaia` module. The query selects stars with non-null parallax, proper motion, and photometry values.

3. **Data Preprocessing**
   - Initial preprocessing includes selecting relevant columns, handling missing values, and calculating new columns to represent physical properties of stars like radial velocity derived from proper motion and parallax.

4. **Exploratory Data Analysis**
   - Visualization of distributions and relationships between features using libraries such as `matplotlib` and `seaborn`. This step is crucial for understanding the data and deciding on the modeling approach.

5. **Feature Engineering and Scaling**
   - Further feature engineering is performed along with scaling of features to prepare the data for machine learning models.

6. **Model Building**
   - Multiple machine learning models are trained, including logistic regression, SVM, decision trees, random forests, and K-nearest neighbors. The models are configured and optimized using techniques such as grid search and cross-validation.

7. **Evaluation**
   - Models are evaluated using metrics like accuracy, precision, recall, F1-score, and ROC curves. A comparison is drawn to select the best model.

8. **ROC Curves and Confusion Matrix**
   - ROC curves for multi-class classification and confusion matrices are plotted to visually assess model performance.

#### Usage
To use this notebook:
1. Ensure all dependencies are installed.
2. Run the notebook cells sequentially to observe the workflow from data fetching to model evaluation.
