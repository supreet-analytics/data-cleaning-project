# 📺 MyAnimeList Data Cleaning Project

This project focuses on cleaning and preparing raw anime data from MyAnimeList for analysis. The dataset contains detailed metadata about various anime series, such as airing dates, ratings, episodes, studios, and more.

---

## 📁 Dataset Overview

- **Source:** [MyAnimeList](https://myanimelist.net/)
- **Format:** CSV
- **Size:** ~18,000 anime entries

---

## 🎯 Objectives

- Clean raw messy data from MyAnimeList
- Extract and format time-based features like `aired_start_date` and `premiered_year`
- Handle missing and inconsistent values
- Prepare dataset for future analysis or modeling

---

## 🧹 Data Cleaning Tasks

- Removed unwanted characters from `aired` column (`{}`, `'`)
- Extracted `aired_start_date` and `aired_end_date` from the `aired` field
- Split `premiered` column into `premiered_season` and `premiered_year`
- Checked for null values using `df.info()` and `isnull().sum()`
- Used log1p() for columns: score, scored_by, members, favorites and duration as these columns where higlhly skewed
- Used Inter Quartile Range (IQR) to detect the number of outliers
- Applied string operations to clean and split columns
- Checked for duplicate records and fixed data types

---

## 🧰 Libraries Used

- `pandas` – data manipulation
- `numpy` – numerical operations
- `matplotlib` & `seaborn` – for visualization: boxplot (to detect outliers)
- `re` – for regex-based string cleaning

---

## 📌 Key Features Engineered

- `aired_start_date`, `aired_end_date`
- `premiered_season`, `premiered_year`

---


## 💡 Learnings

- Handling complex string formats in real-world datasets
- Feature extraction from nested fields
- Standardized cleaning approach for textual and date columns
- Stronger grip on using `pandas` and `regex` for messy data

---

## 📬 Contact

Feel free to reach out if you’d like to collaborate or give feedback!

