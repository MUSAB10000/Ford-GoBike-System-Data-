# Ford GoBike System Data Analysis

This project explores the **Ford GoBike System** dataset, which contains detailed information about individual bike-sharing trips in the San Francisco Bay Area. The analysis is split into two parts: an in-depth EDA notebook and a summarized insights notebook for presentation.

The goal is to uncover patterns in trip durations, user behavior, and how demographic factors like gender and age influence ride patterns.

---

## Dataset Overview

- **Source**: Ford GoBike (February 2019 data)
- **Total Records**: 183,412 trips
- **Features**: 
  - `duration_sec`: trip duration in seconds
  - `start_time`, `end_time`
  - `start_station_name`, `end_station_name`
  - `user_type` (Subscriber or Customer)
  - `member_birth_year`, `member_gender`
  - And station coordinates (lat/long)

---

##  Key Questions Explored

1. What is the distribution of trip durations?
2. How does trip duration vary by user type (Subscriber vs. Customer)?
3. Is there a relationship between demographics (age, gender) and trip duration?
4. How do user type and gender together affect trip patterns?

---

## Exploratory Data Analysis

### Univariate Findings:
- Most trips are **short**, often under 1,000 seconds (~15 minutes).
- **Subscribers** dominate the user base.
- Outliers exist with trips lasting over 40,000 seconds.

### Bivariate Insights:
- **Customers** typically have **longer trips** than Subscribers.
- **No strong correlation** between age and trip duration.

### Multivariate Insights:
- User type has a **stronger effect** on trip duration than gender.
- Longer trips by Customers are consistent across all gender categories.
- Station coordinates show **no clear relationship** with trip length.

---

## Visualizations Included

- Histograms of trip durations (full range and zoomed)
- Box plots comparing trip duration by user type
- Scatter plots of trip duration vs. member birth year
- Facet grids: trip duration by user type and gender
- Pair plots exploring geolocation data vs. duration

---

## Project Structure

- `Part_I_notebook.ipynb`: Full EDA with data wrangling and visualization
- `Part_II_notebook.ipynb`: Summarized version for presentation
---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Conclusion

- The Ford GoBike system is primarily used for **short commutes**.
- **Subscribers** make up the majority of users but have **shorter trips** than **Customers**.
- **Trip durations vary by gender and user type**, but user type is the more influential factor.

---

## License & Credits

This analysis was conducted as part of the **Udacity Data Analyst Nanodegree** program.  
The dataset was provided by **Ford GoBike**.

