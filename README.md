# Will the Customer Accept the Coupon?

## Overview

The goal of this project is to distinguish between customers who accepted a driving coupon versus those that did not.

This project analyses user behavior based on a dataset simulating real-world driving scenarios where coupons are delivered to potential customers. The objective is to understand which factors influence the decision to accept or reject a coupon. The dataset includes attributes such as age, income, time of day, weather, destination and companion type.

## Important Links

[Coupons Dataset](https://github.com/amitkushwaha2000/AIMIL_5.1_Coupon_Acceptance/blob/main/coupons.csv)

[Jupyter Notebook](https://github.com/amitkushwaha2000/AIMIL_5.1_Coupon_Acceptance/blob/main/AIML%205.1%20Coupon%20Analysis.ipynb)

## Data Cleansing 

- All missing values were handled during the cleansing of the dataset. 
  - Dropped the 'car' column due to high missing value ratio.
  - Replaced missing values in the relevant columns (Bar, CoffeeHouse, CarryAway, RestaurantLessThan20 and Restaurant20To50with) with mode imputation.

## Exploratory Data Analysis and Visualizations

- Appropriate visualizations like Bar plots and Pie Charts have been included in the notebook for comparing coupon acceptance rates across age groups, time slots, passenger types etc.
- Multi-category visualizations showing interplay of various factors in deciding acceptance of coupons.

## Key Findings

### Overall Acceptance
- **Overall coupon acceptance rate**: 56.84%
- **Bar coupon acceptance rate**: 41.00%

### Bar Coupons
- Acceptance is higher among those:
  - **Over 25 years old**
  - Who **frequently visit bars**
  - Who are **not traveling with kids**
  - With **higher income** brackets
  - **Not widowed**, and **not in farming/fishing/forestry** occupations
- **Young drivers** (under 30) show higher receptivity.
- **Frequent bar-goers** show significantly higher acceptance rates.

### Coffee House Coupons
- Acceptance is higher among:
  - **Drivers under 30 years**
  - Those traveling with a **friend or partner**
  - Those on trips with **no urgency** or **work-bound** destinations
  - Those who have **previously visited coffee houses**
- **Time of Day** matters: Coupons are more likely accepted during **daylight hours**.
- **Weather sensitivity**: Acceptance is higher in **clear or rainy** conditions and lower in snow.

## Actionable Recommendations

### Segment-Based Targeting
- **Bar Coupons**
  - Focus on individuals **over 25** with **bar visit history**
  - Exclude those with **kids as passengers** or in **farming/forestry occupations**
- **Coffee House Coupons**
  - Prioritize **younger drivers** with **partner/friend passengers**
  - Target **daytime hours**, especially when **weather is sunny or rainy**
  - Focus on those with **prior visits** to coffee houses

## Tools and Libraries Used
- Python 3 (Jupyter Notebook)
- pandas for data analysis
- seaborn & matplotlib for data visualization
- numpy for numerical operations

## Acknowledgments

- UCI Machine Learning Repository for the dataset.
- Amazon Mechanical Turk for survey data collection.
