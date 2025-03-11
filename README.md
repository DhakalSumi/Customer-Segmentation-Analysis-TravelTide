# Customer Segmentation Analysis for TravelTide

## Project Overview
This project aims to enhance customer experiences on TravelTide, a travel and booking platform, by analyzing user behaviors, booking patterns, and engagement trends. By leveraging clustering techniques, we segment customers into distinct groups and tailor personalized offers to improve customer retention and maximize revenue.

## Dataset
The analysis is based on four key tables:
- **Users**: Demographics and user details
- **Sessions**: Online interactions and browsing history
- **Flights**: Booking details for flights
- **Hotels**: Booking details for hotels

## Data Preprocessing
- **Missing Values Handling**: Addressed missing values in `trip_id` and `return_time`.
- **Outlier Removal**: Applied interquartile range (IQR) method to filter extreme values.
- **Data Merging**: Combined all tables into a single dataset for holistic analysis.
- **Feature Engineering**: Created new features such as **booking ratio, engagement period, days since last session, and total spend**.

## Clustering Approach
We applied **K-Means Clustering** to segment users into four groups:
1. **Budget Travelers** – Low engagement, occasional bookers
2. **Business Travelers** – Moderate engagement, frequent bookings
3. **Luxury Travelers** – High spenders with regular bookings
4. **Elite Travelers** – Premium users with maximum engagement and spending

## Model Evaluation
- **Silhouette Score**: Initially low but improved by optimizing clusters and scaling features.
- **Visualization**: PCA was used to reduce dimensions and visualize clusters effectively.

## Business Insights & Recommendations
- **Budget Travelers**: Offer discounts and promotional travel guides.
- **Business Travelers**: Provide loyalty incentives and corporate travel benefits.
- **Luxury Travelers**: Introduce tiered loyalty programs and premium travel perks.
- **Elite Travelers**: Offer exclusive travel packages and VIP concierge services.

## Future Enhancements
- Implement **supervised learning** for customer behavior prediction.
- Use **real-time analytics** to adapt offers dynamically.
- Conduct **A/B testing** to refine personalization strategies.

## How to Run the Project
1. Install dependencies: `pip install -r requirements.txt`
2. Load and preprocess the dataset.
3. Run `clustering_analysis.py` to generate customer segments.
4. Visualize the results using provided scripts.

