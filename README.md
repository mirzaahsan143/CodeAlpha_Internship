<div align="center">
    <img src="https://img.shields.io/badge/Internship-CodeAlpha-blue?style=for-the-badge" alt="CodeAlpha Internship">
    <img src="https://img.shields.io/badge/Topic-Machine%20Learning-orange?style=for-the-badge" alt="Machine Learning">
    <img src="https://img.shields.io/badge/Language-Python-green?style=for-the-badge" alt="Python">
</div>

<h1 align="center">Sales Prediction Using Python</h1>
<h3 align="center">Predicting Sales Based on Advertising Spend Across TV, Radio & Newspaper</h3>

<p align="center">
  <strong>Task Type:</strong> Predictive Analytics / Regression Project <br>
  <strong>Internship Track:</strong> Data Science Tasks
</p>

<hr>

<h2>📋 Project Overview</h2>
<p>
This project focuses on building a predictive model to forecast total sales generated based on the advertising budgets allocated to three main marketing channels: <strong>TV</strong>, <strong>Radio</strong>, and <strong>Newspaper</strong>. By applying exploratory data analysis (EDA), data cleaning, and statistical machine learning tools, this project evaluates business choices and determines which advertising channel provides the optimal Return on Investment (ROI).
</p>

<h2>📊 Dataset Details</h2>
<p>The project utilizes the <code>Advertising.csv</code> dataset downloaded directly from Kaggle using the <code>kagglehub</code> framework. The dataset consists of <strong>200 records</strong> with the following metrics:</p>

<table border="1" cellpadding="8" style="border-collapse: collapse; width: 100%;">
    <thead>
        <tr style="background-color: #f2f2f2;">
            <th>Feature Column</th>
            <th>Data Type</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><strong>TV</strong></td>
            <td>float64</td>
            <td>Advertising budget spent on TV campaigns (in $thousands).</td>
        </tr>
        <tr>
            <td><strong>Radio</strong></td>
            <td>float64</td>
            <td>Advertising budget spent on Radio campaigns (in $thousands).</td>
        </tr>
        <tr>
            <td><strong>Newspaper</strong></td>
            <td>float64</td>
            <td>Advertising budget spent on Newspaper campaigns (in $thousands).</td>
        </tr>
        <tr>
            <td><strong>Sales (Target)</strong></td>
            <td>float64</td>
            <td>Units of product sold (in $thousands) — This is our target prediction variable.</td>
        </tr>
    </tbody>
</table>

<h2>🛠️ Tech Stack & Dependencies</h2>
<ul>
    <li><strong>Programming Language:</strong> Python 3</li>
    <li><strong>Data Manipulation:</strong> <code>pandas</code>, <code>numpy</code></li>
    <li><strong>Data Visualization:</strong> <code>matplotlib</code>, <code>seaborn</code></li>
    <li><strong>Machine Learning Library:</strong> <code>scikit-learn</code></li>
    <li><strong>Statistical Modeling:</strong> <code>statsmodels</code></li>
</ul>

<h2>🚀 Workflow Steps & Technical Explanation</h2>

<h3>1. Data Sourcing and Library Configuration</h3>
<p>All structural frameworks (Pandas, Numpy, Scikit-Learn) are imported. Warnings are suppressed to maintain clean outputs. Plot configurations are standardized to size 10x6 with a <em>whitegrid</em> aesthetic layout for enhanced presentation.</p>

<h3>2. Pre-processing & Robust Data Cleaning</h3>
<ul>
    <li><strong>Missing Value & Duplication Verifications:</strong> Evaluated with zero errors recorded; the dataset contains full values without rows overlapping.</li>
    <li><strong>Outlier Identification (IQR Method):</strong> Calculated boundary metrics across distributions. The checks determined that TV, Radio, and Sales variables were free of anomalies, whereas the Newspaper feature introduced 2 outer data points past the boundary range threshold (Upper boundary: 93.62).</li>
</ul>

<h3>3. Explanatory Plot Analyses (EDA)</h3>
<p>Constructed kernel density evaluations (KDE) alongside standard distribution boxplots to understand the distribution trends of the target column (Sales) and to map feature correlations.</p>

<h3>4. Regression Architecture (Training & Evaluation)</h3>
<p>The records were split into <strong>80% Training</strong> and <strong>20% Testing</strong> folds. Two structural model approaches were constructed and compared side-by-side:</p>
<ol>
    <li><strong>Multiple Linear Regression:</strong> Maps the baseline linear interactions of marketing weight choices.</li>
    <li><strong>Random Forest Regressor:</strong> Introduced as an ensemble method to map complex non-linear combinations across data attributes.</li>
</ol>

<hr>

<h2>📈 Model Evaluation & Key Findings</h2>
<p>Performance calculations yielded the following business insights:</p>

<table border="1" cellpadding="8" style="border-collapse: collapse; width: 100%;">
    <thead>
        <tr style="background-color: #f2f2f2;">
            <th>Evaluated Architecture</th>
            <th>Mean Absolute Error (MAE)</th>
            <th>Root Mean Squared Error (RMSE)</th>
            <th>R² Accuracy Metric</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><strong>Multiple Linear Regression</strong></td>
            <td>~1.26</td>
            <td>~1.40</td>
            <td>~89.8% Variance Captured</td>
        </tr>
        <tr>
            <td><strong>Random Forest Regressor</strong></td>
            <td>~0.62</td>
            <td>~0.71</td>
            <td><strong>~97.5% Variance Captured</strong></td>
        </tr>
    </tbody>
</table>

<h3>🎯 Strategic Conclusions:</h3>
<ul>
    <li><strong>Winner Model:</strong> The <strong>Random Forest Regressor</strong> outperforms baseline structural models, reducing prediction errors by half and validating that budget-to-sales correlations exhibit complex non-linear patterns.</li>
    <li><strong>TV Priority:</strong> Spending on TV is the single most powerful driver of high product sales.</li>
    <li><strong>Synergy Focus:</strong> Radio investments provide excellent efficiency and compound growth when run in tandem with TV spend.</li>
    <li><strong>Newspaper Redirection:</strong> Newspaper ads show weak, non-significant correlations with overall conversions. Marketing budgets should be diverted from Newspaper ads to maximize company revenue.</li>
</ul>

<hr>
<div align="center">
    <p>Completed as part of the CodeAlpha Data Science Internship curriculum.</p>
    <strong>Developed by Mirza Muhammad Ahsan</strong>
</div>
