
# 📊 Netflix Content Analysis using PostgreSQL

![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/inbox_12038776_dbabda1e8f2d39e88b030173303b2724_Netflix.jpg)

## 🎯 Project Objective
This project analyzes Netflix content data using PostgreSQL to derive actionable insights about:
- Content types (Movies vs TV Shows)
- Global content distribution
- Ratings and genres
- Content trends by year and country
- Popular directors and actors
- Thematic categorization based on content descriptions

---

## 🛠️ Tools & Skills Demonstrated

**SQL Functions Used:**
- `RANK()`, `COUNT()`, `UNNEST()`, `TO_DATE()`, `EXTRACT()`, `STRING_TO_ARRAY()`, `ILIKE`

**Techniques Applied:**
- Aggregation and filtering
- Pattern matching and text analysis
- Window functions
- Date-based trend analysis

---

## 📌 Key Queries & Insights

### 1. 🎬 Content Type Breakdown
- Counted the number of **Movies vs TV Shows** to analyze platform focus.

  ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-15%20184638.png)

  ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-15%20184648.png)

### 2. ⭐ Most Common Ratings
- Found the **most frequent rating** by content type using `RANK()`.

  ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-15%20192412.png)

  ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-15%20192432.png)
  

### 3. 📅 Year-Specific Content
- Listed all **movies released in 2020**.

  ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-15%20194408.png)

  ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-15%20194446.png)

  

### 4. 🌍 Top 5 Countries by Content Volume
- Used `UNNEST()` to extract top countries with the most content.

  ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-15%20195959.png)

   ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-15%20200046.png)

  

### 5. 🎥 Longest Movie
- Identified the **longest movie** based on the `duration` field.

![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-16%20160151.png)

![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-16%20160208.png)
  

### 6. 🆕 Recently Added Content
- Filtered content added to Netflix in the **last 5 years**.

![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-16%20161353.png)

![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-16%20161451.png)

### 7. 🎬 Director-Based Search
- Queried all content directed by **Rajiv Chilaka**.

  ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-16%20170110.png)

  ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-16%20170123.png)

### 8. 📺 TV Shows with >5 Seasons
- Used `SPLIT_PART()` to extract season info and filter multi-season shows.

   ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-16%20171119.png)

   ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-16%20171140.png)

### 9. 🎭 Genre Distribution
- Counted the number of titles by **genre** using `UNNEST()` on `listed_in`.

   ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-16%20173242.png)

   ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-16%20173849.png)

### 10. 🇮🇳 India-Specific Trends
- Found **top 5 years** with the highest average content release in **India**.

   ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-16%20175157.png)

   ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-16%20175207.png)

### 11. 🎞️ Documentaries
- Filtered all **documentary movies** using `ILIKE`.
   ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-16%20183147.png)

   ![Image Alt](https://github.com/vasuverma17/netflix_data_analysis_postgresql/blob/main/Screenshot%202025-07-16%20183209.png)

### 12. ❌ Missing Metadata
- Identified content with **missing director information**.

### 13. 🎥 Actor-Focused Analysis
- Movies starring **Salman Khan** in the last 10 years.
- Top 10 actors in **Indian movies** by appearance count.

### 14. 🚫 Content Categorization (Good vs Bad)
- Categorized content as `Bad_Content` or `Good Content` based on keywords like `'kill'` or `'violence'` in the description.

---

## ✅ Recommendations

- Normalize multi-value fields (`country`, `casts`, `listed_in`) for cleaner joins and filters.
- Add **indexes** on `type`, `release_year`, and `country` for better query performance.
- Integrate this analysis with **BI tools** like Power BI or Tableau for visual insights.
- Enhance data quality checks for `NULL` or missing values.

---

## 🧾 Conclusion

This project showcases:
- Proficiency in SQL for real-world content data analysis
- Ability to extract business-relevant insights
- A foundation for further advanced analytics on streaming platforms

---

## 🙏 Thank You

**Created by:** [Your Name]  
**Connect:** [LinkedIn/GitHub/Email]

Feel free to contribute or suggest improvements!
