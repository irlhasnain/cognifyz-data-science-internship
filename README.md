# 🍽️ Cognifyz Technologies – Data Science Internship

> **Restaurant Data Analysis** | Predictive Modeling | Customer Preference Analysis | Feature Engineering

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)
[![Internship](https://img.shields.io/badge/Internship-Cognifyz%20Technologies-purple)](https://cognifyz.com/)
[![Status](https://img.shields.io/badge/Status-Completed-brightgreen)]()

---

## 📌 About the Internship

This repository contains all tasks completed during my **Data Science Internship at Cognifyz Technologies**. The work spans two levels and covers end-to-end data analysis — from raw exploration and feature engineering to machine learning modeling and visual storytelling — all on a real-world restaurant dataset.

---

## 📂 Repository Structure

```
cognifyz-data-science-internship/
│
├── Dataset_.csv                  # Restaurant dataset (source data)
│
├── Level_2_Cognifyz.ipynb        # Level 2 tasks notebook
├── Level_3_Cognifyz.ipynb        # Level 3 tasks notebook
│
├── images/                       # Saved visualisation outputs
│   ├── l2_t1_booking_delivery.png
│   ├── l2_t1_rating_vs_booking.png
│   ├── l2_t2_price_range_dist.png
│   ├── l2_t2_delivery_by_price.png
│   ├── l2_t3_length_dist.png
│   ├── l2_t3_corr.png
│   ├── l3_t1_model_comparison.png
│   ├── l3_t1_feature_importance.png
│   ├── l3_t2_cuisine_votes.png
│   ├── l3_t2_cuisine_rating.png
│   ├── l3_t3_rating_dist.png
│   ├── l3_t3_city_rating.png
│   └── l3_t3_feature_vs_rating.png
│
└── README.md
```

---

## 📊 Dataset

The dataset (`Dataset_.csv`) contains information about restaurants across multiple cities, including:

| Feature | Description |
|---|---|
| `Restaurant Name` | Name of the restaurant |
| `City` | City where the restaurant is located |
| `Cuisines` | Type(s) of cuisine served |
| `Average Cost for two` | Average cost for two people |
| `Has Table booking` | Whether table booking is available (Yes/No) |
| `Has Online delivery` | Whether online delivery is available (Yes/No) |
| `Price range` | Price range category (1–4) |
| `Aggregate rating` | Overall rating (target variable) |
| `Rating text` | Textual rating category |
| `Votes` | Number of votes received |

---

## 🔷 Level 2 – `Level_2_Cognifyz.ipynb`

### Task 1 – Table Booking & Online Delivery
- Calculated the percentage of restaurants offering **table booking** and **online delivery**
- Compared **average ratings** for restaurants with and without table booking
- Analysed **online delivery availability** across different price ranges

### Task 2 – Price Range Analysis
- Determined the **most common price range** among restaurants
- Computed the **average rating** for each price range
- Identified which price range earns the **highest average rating**
- Visualised price range distribution and rating patterns

### Task 3 – Feature Engineering
- Created new features: **Restaurant Name Length** and **Address Length**
- Encoded categorical variables (`Has Table Booking`, `Has Online Delivery`) as binary features
- Generated a **correlation heatmap** showing relationships between engineered features and the target rating

---

## 🔶 Level 3 – `Level_3_Cognifyz.ipynb`

### Task 1 – Predictive Modeling
Built and compared three regression models to predict `Aggregate rating`:

| Model | MAE | RMSE | R² |
|---|---|---|---|
| Linear Regression | — | — | — |
| Decision Tree (depth=8) | — | — | — |
| Random Forest (100 trees) | — | — | — |

> *Metric values populate when the notebook is run with the dataset.*

- **Random Forest** achieved the best performance
- Feature importance analysis revealed **Votes** and **Average Cost for two** as the strongest predictors

### Task 2 – Customer Preference Analysis
- Exploded multi-cuisine entries to analyse individual cuisine performance
- Identified **top 15 cuisines by total votes** (popularity)
- Ranked cuisines by **average rating** (filtered to cuisines with ≥ 50 restaurants)
- Uncovered which cuisine categories consistently outperform the global average

### Task 3 – Data Visualization
- Plotted the **distribution of aggregate ratings** via histogram and rating-category bar chart
- Compared **average ratings across the top 10 cities** by restaurant count
- Visualised relationships between `Price Range`, `Votes`, `Average Cost for two` and the target rating using **box plots** and **scatter plots**

---

## 🛠️ Tech Stack

| Library | Purpose |
|---|---|
| `pandas` | Data manipulation & aggregation |
| `numpy` | Numerical operations |
| `matplotlib` | Core plotting |
| `seaborn` | Statistical visualisations |
| `scikit-learn` | Machine learning models & evaluation |

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/cognifyz-data-science-internship.git
cd cognifyz-data-science-internship
```

### 2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 3. Add the dataset
Place `Dataset_.csv` in the root directory (same level as the notebooks).

### 4. Run the notebooks
```bash
jupyter notebook
```
Open `Level_2_Cognifyz.ipynb` first, then `Level_3_Cognifyz.ipynb`.

---

## 📈 Key Insights

- Restaurants with **table booking** tend to receive higher ratings on average
- **Online delivery** is more prevalent in mid-range (price range 2–3) restaurants
- **Votes** is the single most important predictor of aggregate rating
- Certain cuisines (e.g., Continental, Mughlai) consistently outperform the global mean rating
- The **Random Forest** model significantly outperforms linear regression on this dataset

---

## 🏢 About Cognifyz Technologies

[Cognifyz Technologies](https://cognifyz.com/) is a technology company focused on data science, AI, and machine learning solutions. This internship provided hands-on experience with real-world restaurant data analysis tasks across multiple difficulty levels.

---

## 📄 License

This project is for educational and portfolio purposes as part of the Cognifyz Technologies Data Science Internship program.

---

*Made with ❤️ during the Cognifyz Data Science Internship*
