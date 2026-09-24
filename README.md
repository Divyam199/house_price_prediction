# 🏠 House Price Prediction

## 📌 Question
What factors influence house prices, and can we build a model to 
predict a house's price based on its features (area, bedrooms, 
bathrooms, location, etc.)?

## 📁 Dataset Overview
- Data sourced from Kaggle: [House Price Prediction](https://www.kaggle.com/datasets/shree1992/housedata) by shree1992
- Originally provided as a nested JSON file (`data.dat`), containing 
  4,601 house records
- Key fields: price, bedrooms, bathrooms, sqft_living, sqft_lot, 
  floors, waterfront, view, condition, yr_built, yr_renovated, address
- Some fields required parsing/flattening before use (nested area 
  data, text-encoded room counts)

## 📖 Column Reference

| Column | Meaning |
|---|---|
| `price` | Sale price of the house |
| `bedrooms` | Number of bedrooms |
| `bathrooms` | Number of bathrooms (0.5 = half bathroom, no shower/tub) |
| `sqft_living` | Size of living area in square feet |
| `sqft_lot` | Size of the lot in square feet |
| `sqft_above` | Square footage of the house apart from the basement |
| `sqft_basement` | Square footage of the basement |
| `floors` | Number of floors |
| `waterfront` | 1 = has waterfront view, 0 = does not |
| `view` | 0–4 rating of how good the property's view is (0 = none, 4 = excellent) |
| `condition` | 1–5 rating of the house's overall condition (1 = poor, 5 = very good) |
| `yr_built` | Year the house was originally built |
| `yr_renovated` | Year of last renovation (NaN/0 = never renovated) |
| `date` | Date the house was sold |
| `address` | Property address |

## 🧹 Data Cleaning
- Parsed raw JSON structure into a clean, flat DataFrame
- Extracted `bedrooms` and `bathrooms` from an embedded text string
- Split combined `sqft_living`/`sqft_lot` values into separate 
  numeric columns
- Handled missing/non-standard values (e.g., `yr_renovated`)
- Converted date fields to proper datetime format

## ✅ Data Quality


## 📈 Charts


## 🔑 Key Findings


## 🤖 Price Predictor (Machine Learning)
Built a **Linear Regression** model to predict house price based on 
features such as area, bedrooms, bathrooms, and location.



## 💡 Recommendations


## 🎯 Conclusion


## 🛠️ Tech Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn