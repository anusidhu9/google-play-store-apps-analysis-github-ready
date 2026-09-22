# Google Play Store Apps Analysis

A Python-based exploratory data analysis project using a Google Play Store apps dataset.

## Project Overview

This project explores app information such as:

- App category
- Rating
- Number of reviews
- App size
- Number of installs
- Free vs. paid apps
- Price
- Content rating
- Genres
- Last updated date
- Android version

The analysis includes data inspection, cleaning, feature transformation, missing-value analysis, correlation analysis, visualizations, and category-level comparisons.

## Project Structure

```text
google-play-store-apps-analysis/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── data/
│   └── Play Store Data.csv
│
├── notebooks/
│   └── google-play-store-apps-analysis.ipynb
│
└── outputs/
    └── figures/
```

## Technologies Used

- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook

## Getting Started

### 1. Clone the repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd google-play-store-apps-analysis
```

### 2. Create a virtual environment (recommended)

Windows:

```bash
python -m venv .venv
.venv\Scripts\activate
```

macOS/Linux:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Add the dataset

Place the dataset in:

```text
data/Play Store Data.csv
```

The notebook loads it using:

```python
pd.read_csv("../data/Play Store Data.csv")
```

### 5. Run the notebook

Open VS Code, install the Python and Jupyter extensions, and open:

```text
notebooks/google-play-store-apps-analysis.ipynb
```

Select your Python environment and run the cells from top to bottom.

## Analysis Workflow

The notebook follows this general workflow:

1. Import Python libraries.
2. Load the Play Store dataset.
3. Inspect rows, columns, data types, and descriptive statistics.
4. Clean app-size values and convert them to numeric representations.
5. Clean the installs column and convert installs to integers.
6. Create install-level categories.
7. Clean and convert app prices to numeric values.
8. Examine missing values.
9. Investigate relationships among numeric variables.
10. Analyze ratings, reviews, and installs.
11. Remove duplicate records.
12. Compare app categories using counts, installs, reviews, and ratings.
13. Visualize rating distributions and other relationships.

## Important Note

The notebook is an exploratory analysis rather than a production machine-learning application. Results depend on the version and quality of the dataset placed in `data/`.

## Reproducibility

Run the notebook from the repository using the relative dataset path:

```text
../data/Play Store Data.csv
```

Avoid using a personal computer path such as:

```text
C:/Users/.../Play Store Data.csv
```

This keeps the project portable for teammates and GitHub users.

## Author

Anu Rani

## License

This project is for academic/educational purposes. All rights reserved by the authors.
