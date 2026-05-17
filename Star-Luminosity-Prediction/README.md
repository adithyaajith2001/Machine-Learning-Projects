#  Star Luminosity Prediction using Linear & Polynomial Regression

##  Problem Statement

Stars follow precise physical laws that connect their temperature, radius, and brightness — but these relationships are highly nonlinear and complex.

Given a star's:
- Surface Temperature (Kelvin)
- Radius (relative to the Sun)
- Absolute Magnitude

the goal is to predict its:
- Luminosity (relative to the Sun)

This project builds and compares:

1. **Linear Regression** — baseline model  
2. **Polynomial Regression** — captures nonlinear stellar physics

The nonlinear relationship is inspired by the **Stefan–Boltzmann Law**:

\[
L \propto R^2 T^4
\]

---

##  Why This Matters

Automated luminosity estimation is critical in modern astronomy.

Large sky surveys such as:
- SDSS (Sloan Digital Sky Survey)
- Gaia Mission

catalog millions of stars, making manual calculations impossible at scale.

Machine Learning helps astronomers estimate stellar properties efficiently and accurately.

---

## Machine Learning Framing

This project is framed as a **Supervised Regression Problem**.

### Models Used
- Linear Regression
- Polynomial Regression (Degree 2+)

### Learning Objective
The comparison directly demonstrates one of the most important ML concepts:

- Bias vs Variance Tradeoff
- Underfitting vs Overfitting
- Nonlinear Feature Learning

Polynomial regression captures the nonlinear behavior expected from stellar physics much better than standard linear regression.

---

##  Dataset

**Dataset:** Star Dataset — Kaggle  
- 240 stars
- 7 features

Features used:
- Temperature (K)
- Radius (R/Ro)
- Absolute Magnitude (Mv)

Target:
- Luminosity (L/Lo)

---

## Workflow

### 1. Data Preprocessing
- Data loading using Pandas
- Feature selection
- Train-test split
- Standard scaling
- Log transformation of luminosity

### 2. Exploratory Data Analysis
- Luminosity distribution
- Log-transformed distribution
- Correlation analysis
- Visualization of nonlinear relationships

### 3. Linear Regression
Used as the baseline model for comparison.

### 4. Polynomial Regression
Polynomial features were generated to model nonlinear stellar relationships.

Polynomial degrees were compared to study:
- Underfitting
- Optimal fitting
- Overfitting

### 5. Regression from Scratch
Implemented Linear Regression manually using:
- Gradient Descent
- Weight updates
- Loss minimization

to understand the mathematics behind regression algorithms.

---

## Key Results

### Metrics to Report
- Linear Regression R² Score
- Polynomial Regression R² Score
- RMSE (log-luminosity units)
- Best Polynomial Degree

### Core Insight
> Polynomial regression significantly outperforms linear regression, confirming the nonlinear Stefan–Boltzmann relationship between stellar properties and luminosity.

---

## Visualizations Included
- Luminosity distribution
- Log-luminosity distribution
- Actual vs Predicted plots
- Degree comparison graphs
- Bias-Variance tradeoff analysis

---

## Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab

---

##  How to Run

### Clone Repository
```bash
git clone <your-repo-link>
cd <repo-name>
```

### Install Dependencies
```bash
pip install numpy pandas matplotlib scikit-learn
```

### Run Notebook
Open in:
- Jupyter Notebook
- Google Colab

Run:
```bash
Star's_Luminosity_Prediction.ipynb
```

---

## Learning Outcomes

This project demonstrates:
- End-to-end ML workflow
- Polynomial regression intuition
- Real-world preprocessing
- Feature engineering
- Gradient descent implementation
- Model evaluation and generalization

---



##  Author

**Adithya Ajith**  
Masters in Data Science
Machine Learning & Data Science Enthusiast
