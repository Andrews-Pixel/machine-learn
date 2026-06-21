🔬 Breast Cancer Classification using Logistic Regression
A machine learning project that classifies breast cancer tumors as Malignant (M) or Benign (B) using Logistic Regression on the Breast Cancer dataset.

📌 Project Overview
This project builds a binary classification model to predict whether a breast cancer tumor is malignant or benign based on cell nucleus features extracted from digitized images of fine needle aspirates (FNA).

🗂️ Dataset
Source:Breast Cancer Wisconsin Dataset (`breast-cancer.csv`)
Target Column:`diagnosis` — encoded as `1` (Malignant) and `0` (Benign)
Features: 30 numeric features including radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry, and fractal dimension (mean, standard error, and worst values)
Dropped Column: `id` (irrelevant identifier)

🛠️ Tech Stack
| Library | Purpose |
| `pandas` | Data loading and manipulation |
| `numpy` | Numerical operations |
| `matplotlib` | Data visualization |
| `seaborn` | Correlation heatmap and confusion matrix |
| `scikit-learn` | Model building, scaling, and evaluation |

⚙️ Workflow

1.Load Data — Read CSV into a pandas DataFrame
2.Explore Data — `.head()`, `.shape()`, `.info()`, `.value_counts()`
3.Preprocessing
   - Drop the `id` column
   - Encode `diagnosis`: `M → 1`, `B → 0`
   - Check for null values
4. Correlation Analysis — Compute correlation matrix and visualize with a heatmap; identify highly correlated features (≥ 0.75 with `concave points_worst`)
5.Feature Scaling — Apply `StandardScaler` to normalize features
6.Train-Test Split — 80% training / 20% testing
7.Model Training — Fit `LogisticRegression` on training data
8.Evaluation
   - Accuracy score on test set
   - Training vs. test score comparison
   - Confusion matrix visualization

📊 Results

| Metric | Value |
|---|---|
| Model | Logistic Regression |
| Train Score | `model.score(Train_x, Train_y)` |98.90%
| Test Score | `model.score(Test_x, Test_y)` |98.24%
| Evaluation | Confusion Matrix (TP, TN, FP, FN) |

📁 Project Structure
breast-cancer-logistic-regression/
│
├── Log_reg.ipynb        # Main Jupyter Notebook
├── breast-cancer.csv    # Dataset (add your own copy)
└── README.md            # Project documentation


Prerequisites
pip install pandas numpy matplotlib seaborn scikit-learn


📈 Visualizations
Correlation Heatmap — 20×20 annotated heatmap of all feature correlations
Confusion Matrix — Seaborn heatmap showing Actual vs. Predicted classifications

🙋‍♂️ Author
Andrews Martin
LinkedIn: [linkedin.com/in/andrewsmartin30](https://linkedin.com/in/andrewsmartin30)
