# ✈️ Flight Data Analysis — EaseMyTrip Dataset

## 📘 Introduction
This project focuses on analyzing a **flight booking dataset** obtained from the [EaseMyTrip](https://www.easemytrip.com/) website.
The main objective is to extract meaningful insights using **statistical analysis and visualization**, and to train a **Linear Regression** model for predicting flight prices.

EaseMyTrip is an Indian online platform for flight booking. By analyzing real-world flight booking data, we aim to uncover patterns and relationships that can help passengers and travel businesses make informed decisions.

---

## 🎯 Research Questions

The study aims to answer the following questions:
1. ✈️ Does **price vary with Airlines**?
2. 🕒 How is **price affected when tickets are booked 1–2 days before departure**?
3. 🌆 How does **price change with Source and Destination cities**?

---

## 🧮 Data Collection and Methodology

- **Data Source:** [EaseMyTrip](https://www.easemytrip.com/) (scraped using **Octoparse** tool)
- **Data Type:** Secondary data (scraped online)
- **Collection Period:** February 11 – March 31, 2022 (50 days)
- **Total Records:** 300,261 unique flight booking options
- **Class Categories:** Economy and Business
- **Dataset Origin:** [Kaggle - EaseMyTrip Flight Price Dataset](https://www.kaggle.com/)

Data was cleaned and preprocessed to ensure consistent formatting and accuracy.

---

## 📊 Dataset Overview

| Column Name | Description |
|--------------|-------------|
| **Airline** | Name of the airline (6 unique airlines) |
| **Flight** | Unique flight code |
| **Source City** | Departure city (6 metro cities) |
| **Departure Time** | Time category for departure |
| **Stops** | Number of stops (Non-stop, 1-stop, 2+ stops) |
| **Arrival Time** | Time category for arrival |
| **Destination City** | Arrival city (6 metro cities) |
| **Class** | Seat class — Business or Economy |
| **Duration** | Flight duration in hours |
| **Days Left** | Days between booking and departure |
| **Price** | Target variable — ticket price (in INR) |

---

## 🧰 Tools & Libraries Used

- **Python** 🐍
- **NumPy** → Numerical computations
- **Pandas** → Data manipulation
- **Matplotlib** & **Seaborn** → Data visualization
- **Octoparse** → Web scraping

---

## 🧹 Data Cleaning Steps

- Removed redundant columns like `index`.
- Verified data types and missing values.
- Ensured consistency in categorical labels.
- Separated Economy and Business class data when required.

---

## 🔍 Exploratory Data Analysis (EDA)

Key visualizations and findings:

1. **Airline Frequencies** — Horizontal bar chart showing flight count per airline.
2. **Departure vs Arrival Time** — Distribution of flights across time intervals.
3. **Source vs Destination Cities** — Comparison of flight frequencies between metro cities.
4. **Price Variation by Airline & Class** — Bar plots showing how business and economy prices differ per airline.
5. **Effect of Booking Time** — Analysis of how ticket prices increase as departure nears.
6. **Price vs Route** — Relationship between price, source city, and destination city.

---

## 📈 Statistical & Predictive Analysis

- Implemented **Linear Regression** to predict the continuous variable `price`.
- Explored relationships between categorical variables and target feature.
- Observed patterns such as:
  - Business class tickets are significantly costlier across all airlines.
  - Prices surge when booked closer to departure.
  - Certain routes (like Delhi–Mumbai) are consistently higher priced due to demand.

---

## 💡 Insights

- **IndiGo** and **Air India** dominate the dataset in terms of flight frequency.
- **Business Class** fares are consistently 2–4× higher than **Economy Class**.
- **Booking early** (≥15 days) results in much cheaper tickets.
- **Evening flights** tend to have higher prices due to demand.
- **Metro–Metro routes** like Delhi–Mumbai, Bangalore–Delhi have higher average fares.

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/Gyanusahu/Flight_Data_Analysis.git
   cd Flight_Data_Analysis
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Open and run the notebook or Python script:
   ```bash
   jupyter notebook
   ```
   or  
   ```bash
   python flight_analysis.py
   ```

---

## 📂 File Structure

```
Flight_Data_Analysis/
│
├── flights_data.csv               # Dataset
├── flight_analysis.ipynb          # Analysis notebook
├── README.md                      # Project documentation
└── requirements.txt               # Dependencies
```

---

## 🧠 Future Work

- Add **machine learning models** like Random Forest, XGBoost for price prediction.
- Implement **feature importance** analysis for deeper insights.
- Build a **dashboard** for interactive visualization using Plotly or Streamlit.

---

## 👨‍💻 Author

**Gyanu Sahu**  
📧 [gyanusahu@gmail.com](mailto:gyanusahu@gmail.com)  
🔗 [GitHub: Gyanusahu](https://github.com/Gyanusahu)
