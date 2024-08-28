# 15-kV Class XLPE Cable Analysis

## Overview

This project aims to analyze the health and condition of 15-kV Class XLPE underground cables using a dataset that tracks various parameters over different inspection years. The dataset includes key features such as cable age, partial discharge levels, visual condition, neutral corrosion, loading, and an overall health index. The analysis is designed to help understand the relationships between these parameters, identify potential issues with cable aging, and provide insights for maintenance planning.

## Why This Project?

Underground cables are critical components of electrical distribution networks, and their reliability is crucial for maintaining uninterrupted power supply. Over time, these cables can degrade due to various factors such as partial discharge, corrosion, and mechanical stress. Understanding how these factors influence the overall health of the cables can help in predictive maintenance, ultimately reducing the risk of cable failures and improving network reliability.

## Dataset Description

The dataset consists of 2,500 records with the following columns:

- **ID**: Unique identifier for each cable segment.
- **Age**: The age of the cable in years at the time of inspection.
- **Partial Discharge**: A normalized value indicating the extent of partial discharge within the cable insulation, which can signify insulation degradation.
- **Visual Condition**: A qualitative assessment of the cable's physical condition, categorized as "Good," "Medium," or "Poor."
- **Neutral Corrosion**: A normalized value indicating the level of corrosion on the cable’s neutral, affecting the cable’s conductivity and longevity.
- **Loading**: The recorded peak loading in Amps, representing the highest current the cable has carried.
- **Health Index**: A score indicating the overall health of the cable, on a scale from 1 (Poor) to 5 (Good).

## Data Analysis

### Visualizations

- **Pie Chart of Visual Condition**: Shows the distribution of cable segments across different visual condition categories.
  
- **Histograms**: Display the frequency distribution of Partial Discharge, Loading, and Neutral Corrosion values.
  
- **Scatter Plots**: Explore relationships between key parameters, such as:
  - Partial Discharge vs. Loading
  - Partial Discharge vs. Neutral Corrosion
  - Loading vs. Neutral Corrosion

- **Box Plots**: Visualize the presence of outliers in Partial Discharge, Neutral Corrosion, and Loading.

- **Correlation Heatmap**: Reveals correlations between numerical variables, helping to identify potential dependencies and interactions.

### Key Insights

1. **Age and Partial Discharge**:
   - Older cables tend to have higher levels of partial discharge, likely due to insulation degradation over time.
  
2. **Age and Neutral Corrosion**:
   - Corrosion levels generally increase with the age of the cable, impacting the overall health and reliability.

3. **Loading and Health Index**:
   - Higher loading tends to correlate with lower health indices, indicating that heavily loaded cables are more prone to deterioration.

### Outliers Detection

- **Partial Discharge, Neutral Corrosion, and Loading**:
  - No significant outliers were detected in the dataset for these parameters, indicating that the values are within expected ranges.

## Time Series Creation

A time series was generated by calculating the installation year of each cable (based on age) to analyze trends over time.

## Interactive Dashboard

Below is an embedded interactive Tableau dashboard that visualizes the key findings from the analysis. The dashboard allows you to interact with the data and explore various aspects of the cable health assessment.

![Screenshot 2024-08-27 230447](https://github.com/user-attachments/assets/0699373a-5cc6-43b2-9544-2ab5ed4604a6)

https://public.tableau.com/views/CABLEHEALTH/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

## Conclusion

This analysis provides a foundational understanding of the factors affecting the health of underground 15-kV Class XLPE cables. By visualizing and correlating these factors, maintenance teams can better predict potential failures and prioritize inspections, leading to more effective maintenance strategies.

## Future Work

Future analysis could involve more sophisticated modeling techniques to predict cable failures based on historical data, possibly incorporating machine learning models to improve predictive maintenance practices.

## Requirements

To run the analysis, you'll need the following Python libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`

## How to Use

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/15-KV-XLPE-Cable-Analysis.git
pip install -r requirements.txt

### Instructions:
1. **Replace** the GitHub repository link (`https://github.com/yourusername/15-KV-XLPE-Cable-Analysis.git`) with the actual link to your repository.
2. **Copy and paste** this content into a `README.md` file in your GitHub repository.
3. **Commit and push** the file to your repository to make it live.
