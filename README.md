# 📊 Netflix Movies & TV Shows Analysis (Power BI)

This project analyzes all the movies and TV shows added to Netflix over the years, uncovering content trends, ratings, genres, and geographical distribution.  
The dataset was sourced from Kaggle: [Netflix Movies and TV Shows](https://www.kaggle.com/datasets/anandshaw2001/netflix-movies-and-tv-shows).

---

## 📂 Dataset Information
The dataset includes the following columns:

| Column        | Description |
|--------------|-------------|
| **show_id**   | Unique identifier for each title (e.g., s1, s2). |
| **type**      | Whether the title is a *Movie* or a *TV Show*. |
| **title**     | Name of the title. |
| **director**  | Director of the title. |
| **cast**      | Main actors involved. |
| **country**   | Country of production. |
| **date_added**| Date when the title was added to Netflix. |
| **release_year** | Year of original release. |
| **rating**    | Content rating (e.g., PG-13, TV-MA). |
| **duration**  | Duration in minutes (for movies) or seasons (for shows). |
| **listed_in** | Categories or genres. |
| **description** | Brief summary. |

---

## 🔧 Data Modeling
- Columns like **country**, **genre**, **director**, and **cast** were split and unpivoted to create **separate dimension tables** for detailed filtering.  
- The model contains **many-to-many relationships**, but with **cross-filter direction** enabled, the visuals work seamlessly.

![Data Model](https://github.com/divyamehulmakwana-bit/Netflix-Analysis-using-PowerBi/blob/main/screenshots/Model.png)

---

## 📈 Dashboard Overview
The Power BI report is divided into **three pages**:

### 🔹 1. Summary Page
- KPIs:  
  - **Total Titles:** ~9K  
  - **Total Genres:** 43  
  - **Oldest Title:** 1925  
  - **Newest Title:** 2021  
  - **Total Countries:** 123  
- Visuals:  
  - Top 5 Directors (Rajiv Chilaka leads with 22 titles)  
  - Content Ratings Distribution (TV-MA most common)  
  - World Map of Content Origin (USA & India lead)  
  - Movie vs. Show Distribution (69.6% Movies, 30.4% Shows)  

![Summary Page](https://github.com/divyamehulmakwana-bit/Netflix-Analysis-using-PowerBi/blob/main/screenshots/Summary%20Page.png)

---

### 🔹 2. Movies Page
- Added KPI: **Avg Movie Length (~100 mins)**  
- Visuals:  
  - Top Producing Countries (USA & India dominate)  
  - Movie Duration Distribution (Most 50–70 mins)  
  - Top Movie Actors  
  - Movies Added Over Time (2019 peak)  
  - Genre Treemap (Drama, Comedy, Documentary)  

![Movies Page](https://github.com/divyamehulmakwana-bit/Netflix-Analysis-using-PowerBi/blob/main/screenshots/Movies%20Page.png)

---

### 🔹 3. Series Page
- Added KPI: **Avg Seasons (~2 seasons)**  
- Visuals:  
  - Country-wise Distribution  
  - Longest Running Shows (Grey’s Anatomy – 17 seasons)  
  - Top Show Actors  
  - Genre Funnel (TV Drama, Comedy lead)  
  - Shows Added Over Time  

![Series Page](https://github.com/divyamehulmakwana-bit/Netflix-Analysis-using-PowerBi/blob/main/screenshots/Series%20Page.png)

---

## 🛠️ Tech Stack
- **Power BI** – Data cleaning, modeling, and visualization  
- **Excel / Power Query** – Data preprocessing  
- **Kaggle Dataset** – Source of Netflix data  

---

## 🚀 Key Insights
- **Movies dominate Netflix’s library** (~70%).  
- **2019 was a peak year** for new titles added.  
- **Drama & Comedy** are the most popular genres.  
- **USA and India** lead in content production.  
- Many titles have **TV-MA rating**, showing a mature content trend.

---

## 📌 How to View
You can explore the full Power BI report by cloning this repo:  
```bash
git clone https://github.com/divyamehulmakwana-bit/Netflix-Analysis-using-PowerBi.git
