# Black-Friday-Macro-Trend-Analysis
Using Python and statistical correlation models to decode retail datasets, optimize discount strategies, and visualize market share.

# 1. Project Objectives
The goal of this project was to figure out what actually drives consumer spending. Specifically, I wanted to use the data to answer a few core questions:

Which product categories actually perform the best?

Do bigger discounts actually lead to more sales revenue?

Which customer segments are spending the most money?

What time of day do purchases peak?

How does purchasing behavior change from city to city?

# 2. Methodology
To answer these questions, I analyzed the raw dataset using Python (Pandas, Matplotlib, and Seaborn). Here is how I broke it down:

Cleaning the Data: First, I audited the dataset to make sure it was reliable. I checked for null values, missing entries, and duplicates to ensure the data was clean before running any math on it.

Ranking Categories: I used Pandas groupby to aggregate the data and built a bar chart to rank the top product categories. While there was a clear winner, the visual showed that the margins between the top categories were actually surprisingly tight.

Finding the Drivers (Correlation): To figure out how different variables interact, I generated a correlation matrix and visualized it with a Seaborn heatmap. My main goal here was to test if there is an actual mathematical correlation between discounts and sales revenue (which I break down in the findings below).

Mapping the Customers: I grouped the spending data and used a pie chart to get a clear visual of which demographic segments hold the most purchasing power.

Timing the Market: Using the value_counts function on the timestamps, I was able to pinpoint exactly what time of day transactions peak.

# 3. Key Business Insights
Insight 1: The Reality of Discounts

The Finding: The data shows no meaningful relationship (r = -0.10) between how much we discount an item and how much a customer ultimately spends. Because deeper discounts aren't translating to higher revenue, we can safely reduce our promotional offers to protect baseline margins.

Insight 2: Sales are almost identical across all cities

The Finding: At first glance, four cities technically fell below our average. However, looking at the standard deviation, the gap between the lowest city (LA at 9,719) and the highest (NY at 10,105) is so small it is basically statistical noise. Geography isn't a factor People are buying at the exact same rate no matter where they live.

Insight 3: The company is great at acquiring customers, but terrible at keeping them

The Finding: The data shows that our ads are doing exactly what they are supposed to do: just over 30% of our shoppers are brand new. However, only 10% of our customers make it to VIP status, and just 25% are considered loyal. This tells us we are great at getting people to buy for the first time, but we struggle to turn them into long-term fans.

# 4. Strategic Recommendations

Recommendation 1:To protect profit margins, we should dial back the heavy discounts.

Recommendation 2: Because the sales numbers are so flat across different cities, we shouldn't spend the extra money running local, geotargeted ads to fix lower-performing areas. A buyer in LA is acting exactly like a buyer in New York. We should just run broad, national campaigns and focus on what they are buying, rather than where they live.

Recommendation 3: Since the ads are working well to bring people in, we shouldn't change much there. Instead, we need to figure out why people aren't sticking around. We should review the VIP rewards program to make sure the perks are actually exciting enough to convince a first-time buyer to come back.













Geographic Breakdown: Finally, I filtered the geographic data to isolate the bottom 5 cities to see where sales were underperforming the most.
