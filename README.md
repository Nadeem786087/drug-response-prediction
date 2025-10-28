# Gene Expression vs Drug Sensitivity (Linear Regression)

This project demonstrates how gene expression data can be used to predict drug sensitivity (IC50 values) using a simple linear regression model. The dataset is synthetic and meant for educational purposes in bioinformatics and machine learning.

---

## Step-by-Step Workflow

### Step 1: Import Libraries
We imported essential Python libraries like **pandas**, **numpy**, **matplotlib**, and **scikit-learn** for data handling, visualization, and modeling.

### Step 2: Create a Synthetic Dataset
A toy dataset was created showing an **inverse relationship** between gene expression and IC50 values:

- **GeneY_Expression** → Predictor variable (normalized)
- **IC50_nM** → Target variable (drug sensitivity)

### Step 3: Visualize Data
A scatter plot was used to confirm a **negative linear trend** — higher GeneY expression leads to lower IC50 values, meaning greater drug sensitivity.

### Step 4: Prepare Data for Model Training
We split the dataset into:
```python
X = df[["GeneY_Expression"]]  # Feature  
y = df[["IC50_nM"]]           # Target
```

### Step 5: Train a Linear Regression Model
A **LinearRegression** model from `scikit-learn` was trained to learn the relationship.

### Step 6: Visualize the Model
We used multiple plots to evaluate the model:

- **Regression Line Plot:** shows the fitted linear trend  
- **Residual Plot:** residuals scattered evenly → good model fit  
- **Predicted vs Actual Plot:** near-perfect alignment → high accuracy  

### Step 7: Make Predictions
Predicted IC50 for a new cell line with **GeneY expression = 5.5**:

```python
Predicted IC50 ≈ 52.38 nM
```

### Step 8: Summary
Our analysis shows a clear **inverse linear relationship** between gene expression and IC50 values.  
Higher **GeneY expression** → lower **IC50**, indicating increased drug sensitivity.

---

##  Key Learning Outcomes
- How to create and explore a synthetic bioinformatics dataset.  
- How to train and visualize a simple linear regression model.  
- How gene expression levels can relate to drug response metrics.

---

## Tools & Libraries
- Python 3  
- pandas  
- matplotlib  
- scikit-learn  

---

## Repository Structure
```
├── gene_expression_drug_sensitivity.ipynb   # Jupyter Notebook
├── README.md                                # Project overview
```
