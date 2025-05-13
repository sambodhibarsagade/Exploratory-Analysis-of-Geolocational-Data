# 🛰️ GeoStay – Optimized Accommodation Suggestions Using Geolocational Machine Learning

> A machine learning-based system for helping students and urban planners make smarter housing decisions using geolocation data and clustering.



##  Table of Contents

- [Overview](#-overview)
- [Objective](#-objective)
- [Problem Statement](#-problem-statement)
- [Technical Framework](#-technical-framework)
- [System Architecture](#-system-architecture)
- [Results](#-results)
- [Benchmarking](#-benchmarking)
- [Societal Impact](#-societal-impact)
- [Future Scope](#-future-scope)
  



##  Overview

Every year, millions of students move to new cities or countries for higher education — and finding the right accommodation is a major challenge. Platforms like Airbnb or Zillow provide listings but often fail to consider what's truly important for students: affordability, proximity to campus, and access to nearby amenities.

**GeoStay** is a project designed to solve this problem by combining **machine learning**, **geolocation APIs**, and **visualization tools** to make accommodation suggestions more personalized, relevant, and smart.


##  Objective

- Analyze geolocation data to form meaningful housing clusters.
- Use **K-Means** and **PCA** to reduce noise and highlight useful groupings.
- Integrate **real-time REST APIs** for amenity data (e.g., hospitals, shops).
- Visualize the clusters using interactive maps and charts.
- Validate recommendations based on lifestyle and income-based preferences.



##  Problem Statement

### Current Challenges:
-  Traditional systems often achieve ≤65% satisfaction.
-  Geolocation data is sparse or outdated.
-  No personalization for income-based lifestyles or safety preferences.

### GeoStay’s Solution:
-  **Hybrid Clustering** using K-Means + PCA.
-  **Real-Time API Updates** to keep data fresh.
-  **Student-Centric Clusters** based on budget, distance from college, and amenities.



##  Technical Framework

### Algorithms:
- **K-Means Clustering**: Optimized using the **Elbow Method** (best K = 4).
- **PCA**: Used for dimensionality reduction (87.3% variance retained).
- **APIs**: Used to fetch real-time location data on surrounding services.

### Libraries & Tools:
- Python, Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib
- Folium (for map visualization)
- Google Places API or similar



##  System Architecture

1. **Input**: Accommodation dataset with geolocation, rent, and amenity info.
2. **Preprocessing**: Clean and standardize the data.
3. **Clustering**: Apply K-Means with Elbow method.
4. **PCA**: Reduce dimensionality for better clustering and visualization.
5. **API Integration**: Get updated nearby places every 24 hours.
6. **Visualization**: Plot results using Folium and Seaborn.
7. **UI**: Login-based system to let users view tailored results.



##  Results

### Cluster Highlights:
- **Cluster 1 (Premium)**: <1 km from college, 15+ nearby amenities.
- **Cluster 2 (Budget)**: 2–4 km range, 5–7 amenities.
- **Others**: Represent different budget and distance combinations.

### Performance:
-  **F1-score**: 92.4% (via 10-fold cross-validation)
-  **User Satisfaction**: 85% (based on survey of 120 students)



##  Benchmarking

- Outperformed traditional filtering systems.
- Offers real-time, actionable insights.
- Dynamic clustering based on both **static data** and **live API feeds**.



##  Societal Impact

-  Students: Find housing faster and smarter.
-  Planners: Identify areas lacking essential services.
-  Businesses: Discover ideal locations for opening near student zones.



##  Future Scope

-  Add **ARIMA** models for rent trend forecasting.
-  Use **NLP** to analyze reviews for safety & comfort.
-  Expand globally with support for international university hubs.
-  Add **transport API** integration for commute mapping.
-  Explore voice-based search using assistant tools.





## 📎 References

- Voumick, Deb, Sutradhar — *Online Based Smart House Renting* (2021)  
- S. G. K. Patro et al. — *HAR-KNN Recommendation System* (IEEE, 2020)  
- M. Sumithra — *Exploratory Analysis of Geo-Location Data* (2022)



