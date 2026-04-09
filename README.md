# User Behavior Analysis & Purchase Prediction Dashboard

## Project Overview
This project analyzes a dataset of 8,000 user sessions to identify patterns leading to purchases and to detect potential bottlenecks in the conversion funnel. Despite a high overall conversion rate (99.8%), the analysis focuses on segmenting user behavior and identifying technical/UX issues for the remaining 0.2%.

## Key Insights
- **The Engagement Paradox:** The `Adult` group on `Mobile` devices shows the highest conversion efficiency with the lowest `Engagement Index`. This suggests a highly optimized mobile path-to-purchase for this demographic.
- **Technical Drop-off:** Non-purchasers (0.17%) exhibit a `Bounce Rate` > 90%, primarily on mobile devices. This points toward a potential technical issue or slow loading times for specific mobile segments.
- **Customer Loyalty:** High average of previous purchases (~6.9) across all segments indicates strong brand retention and repeat customer value.

## Visualizations Included
1. **Conversion KPI Card:** Real-time tracking of purchase rates.
2. **Behavioral Matrix:** Cross-analysis of Device Type and Age Groups against previous purchases and engagement.
3. **Decomposition Tree:** An AI-powered path analysis showing the most significant influencers for completed purchases.
4. **Engagement vs. Conversion Line Chart:** Visualizing the correlation between session depth and final conversion.

## Tech Stack & Data Engineering
- **Power Query (M):** 
  - Data cleaning and normalization.
  - Feature Engineering: Created `Age Groups` (Young, Adult, Senior).
  - Handled missing values by replacing nulls with "Unknown" for categorical data.
- **DAX Measures:**
  - `Conversion Rate`: `%` of successful purchases.
  - `User Engagement Index`: A weighted score based on `time_on_site` and `pages_viewed`.
  - `Avg Pages per Minute`: Efficiency metric for user sessions.

## How to View
1. Download the `User_Behavior_Analysis.pbix` file.
2. Open with [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
3. (Optional) View the PDF summary in the `/exports` folder.
