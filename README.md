## Airbnb-EDA

![1624110814273](https://github.com/user-attachments/assets/3b684f6f-037f-483c-9188-8dfb96d7d9f7)

### Project Overview

In this project I have completed Explanortory Data Analysis for New York Airbnb data to understand the renting pattern.
I have used **Pandas** for filtering and aggregating, **Matplotlib and Seaborn** for visualisation. 

### Objectives 
1. Analyze **room types, prices, and availability** across different neighborhoods.
2. Understand **host behavior** and listing patterns.
3. Detect potential **outliers** in prices.
4. Provide recommendations for guests and hosts based on insights.
---

### Dataset 

I have used the dataset from Kaggle which contains 20,756 listings and 22 columns. 

Link to dataset - https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data
- **id**: Unique identifier for each listing  
- **name**: Title of the Airbnb listing  
- **host_name**: Name of the host  
- **neighborhood_group**: Group (borough) where the listing is located  
- **latitude/longitude**: Geolocation of listings  
- **price**: Nightly rental price  
- **room_type**: Type of accommodation (e.g., entire home, private room)  
- **reviews_per_month**: Average monthly reviews for the listing  
- **availability_365**: Number of available days in the year
---

### WorkFlow 
**1. Data Cleaning**
- Handled missing data: price, neighbourhood, bed has null values.
- Fix data types: Converted `last_review` to a datetime object.
- Remove outliers Listings with prices > $1,000 were capped to avoid skewed visualizations.

**2. EDA Explanototy Data Analysis**
1. **Room type distribution**: 
   - Visualized the count of each room type using **bar plots**.
   - Identified **Entire home/apt** as the most common room type.

2. **Neighborhood group insights**:
   - Analyzed **price variations by boroughs**.
   - Manhattan had the **highest average prices**.

3. **Availability trends**:
   - Used **heatmaps** to show correlations among `price`, `availability_365`, `number_of_reviews`, and `beds`.

4. **Price distribution**:
   - Used **histograms** to show the distribution of prices.
   - Majority of the listings were priced between **$50 - $300**.

5. **Host listings**:
   - Analyzed hosts with multiple listings using **boxplots** to identify key contributors.

6. **Review behavior**:
   - Used **pair plots** to show relationships between number of reviews, price, and availability.

**3. Data Visualization**
- **Pairplot**: To see correlations among `price`, `availability`, and `number of reviews`.
- **Heatmap**: Showing correlations among numerical features.
- **Histograms and Boxplots**: To detect outliers in `price`.
- **Bar Charts**: Displaying room types and neighborhood group distributions.

---
## Conclusion
This project offers valuable insights into the New York Airbnb market, helping both guests and hosts make informed decisions. By using **EDA techniques**, we identified key trends and developed actionable recommendations. 
