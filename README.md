# Smartphone Market Analysis 

This project analyzes sales and pricing trends in the mobile phone market using Python and popular data visualization libraries like Matplotlib, Pandas, Numpy, and Seaborn. The goal is to extract actionable insights regarding product features, pricing strategies, and sales performance. By leveraging data analysis techniques, this project identifies key trends and patterns that can guide market strategies.

Project Objective :

The primary objective of this project is to:

- Analyze sales and pricing trends in the mobile phone market.

- Evaluate critical product features, including display technology (e.g., LED, LCD, OLED), resolution, and dimensions.

- Organize data for efficient product comparisons.

- Identify effective pricing strategies and insights to optimize market performance.

Features and Methodology :

1. Data Loading and Cleaning

- Dataset: The project uses a CSV file (processed_data2.csv) containing sales data for mobile phones.

- Initial exploration and cleaning steps ensure the data is suitable for analysis.

  import pandas as pd
  df = pd.read_csv("processed_data2.csv")
  print(df.head())

2.Sales and Pricing Trends :

- Visualized pricing trends over time and analyzed correlations between product features and sales performance.

- Example: Trend of average prices for various display technologies.

  import matplotlib.pyplot as plt
  sns.lineplot(data=df, x="Year", y="Average Price", hue="Display Technology")
  plt.title("Pricing Trends by Display Technology")
  plt.show()

3.Feature Comparison :

- Compared mobile phone features (e.g., resolution and dimensions) to evaluate their impact on pricing and sales.

  sns.boxplot(data=df, x="Resolution", y="Price")
  plt.title("Price Distribution by Resolution")
  plt.show()

4.Insights and Findings :

- Identified optimal price ranges for different product categories.

- Analyzed feature-specific trends, such as the popularity of OLED displays over LCD in recent years.

Conclusion :

This project demonstrates the utility of Python in visualizing and analyzing complex datasets. The analysis highlights:

- Key product features influencing sales and pricing.

- Trends that can help businesses strategize their offerings in a competitive market.

By providing clear visualizations and actionable insights, this project serves as a foundation for data-driven decision-making in the mobile phone industry.

How to Run the Project:

1. Clone the repository:

   git clone https://github.com/suryani763/mobile-market-analysis.git
