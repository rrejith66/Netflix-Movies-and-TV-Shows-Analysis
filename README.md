# 📺 Netflix Data Cleaning & Preprocessing

This project focuses on cleaning, preprocessing, and performing preliminary exploratory analysis on a dataset containing metadata about Netflix content. The goal is to prepare the dataset for insightful visualizations, storytelling, and future modeling work.

---

## 📂 Dataset Overview

The dataset consists of metadata about Netflix's content such as:

- **Title, Type** (Movie/TV Show)
- **Director, Cast, Country**
- **Date Added to Netflix**
- **Release Year**
- **Rating** (e.g., PG, TV-MA)
- **Duration**
- **Genres** (Listed In)
- **Description**

> 📌 **Total Records:** 8,790  
> 📌 **Source:** Public dataset available via [Kaggle](https://www.kaggle.com/shivamb/netflix-shows)

---

## 🧹 Data Cleaning & Preprocessing

Key cleaning steps performed:

- ✅ **Handled Missing Values**:
  - Filled `director`, `cast`, and `country` with `'Unknown'` or `'Not Available'`
  - Parsed and filled `date_added` with proper datetime format

- ✅ **Datetime Conversion**:
  - Converted `date_added` to `datetime64[ns]`
  - Extracted `year_added`, `month_added`, `day_of_week_added` from `date_added`

- ✅ **Standardized Text Columns**:
  - Removed leading/trailing spaces
  - Converted case using `.str.lower()` or `.str.title()`

- ✅ **Feature Engineering**:
  - Split `duration` into `duration_minutes`
  - Identified and isolated content trends by type, genre, and geography

---

## 📊 Key Insights

- **Movies** dominate the Netflix catalog compared to TV Shows
- Most content was added between **2018–2020**
- **Drama, Comedy**, and **International Movies** are the most common genres
- Content originates mainly from the **United States**, followed by **India**
- **TV-MA** and **TV-14** are the most frequent content ratings

---

## 🚀 Future Enhancements

- Perform in-depth EDA & visualization
- Build an interactive dashboard (Power BI, Tableau, or Plotly)
- Use this cleaned dataset for predictive modeling (e.g., content success prediction)
- Integrate genre clustering or recommendation systems

## 🙌 Acknowledgements
- Netflix Inc. (for content inspiration)
- Kaggle Dataset
