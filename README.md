# Sales_distribution

📊 **Sales Data Distribution Analysis**

This project explores the distribution characteristics of a retail sales dataset using Python-based statistical and visual methods. The goal is to understand key patterns in sales, pricing, quantity, discount behavior, and regional trends through various distribution tests.

🔍 **Key Objectives**

Perform statistical distribution tests (Shapiro-Wilk, Skewness, IQR).

Understand how Sales_Amount, Unit_Price, and other features behave across various dimensions like region and customer type.

Compare different theoretical distributions (Normal, Exponential, Log-Normal) for model fitting.

Identify outliers using the IQR method.

Visualize and interpret data to guide business insights.

📌 **Dataset Highlights**

10+ columns of clean, structured sales data.

Covers multiple regions and product categories.

Differentiates between new and returning customers.

📈 **Techniques Used**

Pandas, NumPy for data handling.

Seaborn, Matplotlib for visual exploration.

SciPy for distribution tests (Shapiro-Wilk, Log-Normal fitting).

Exploratory analysis using histograms, boxplots, and distribution comparisons.

🛠️ **Tools & Libraries**

Python: pandas, numpy, matplotlib, seaborn, scipy

Jupyter Notebook: for running and visualizing exploratory code

🧪 **Key Insights**

📊 Q1: Is Sales_Amount Normally Distributed?

Shapiro-Wilk Test p-value: 0.0000 → Not Normal
Interpretation: The sales amounts do not follow a normal distribution. Further analysis should use non-parametric or distribution-agnostic methods.

📊 Q2: What is the Skewness of Unit_Price?

Skewness = 0.02 → Right-Skewed
Interpretation: Unit_Price is very slightly right-skewed, but close to symmetric.

📊 Q3: Is Quantity_Sold Uniformly Distributed?

Not Uniform. Most values cluster between 10–40.

Interpretation: Sales quantities are not equally likely; customers tend to purchase in small to mid-sized quantities.

📊 Q4: Is Discount Unimodal or Bimodal?

Unimodal with concentration in the 0.10–0.20 range.

Interpretation: Suggests a consistent discounting policy in place (e.g., common thresholds like 10%, 15%, 20%).

📊 Q5: How Does Unit_Cost Vary by Product Category?

Electronics & Furniture → Higher costs, wider range

Clothing & Food → Lower and more consistent

Interpretation: Product categories show expected cost differences, useful for cost analysis and pricing strategy.

📊 Q6: Does Sales_Amount Distribution Vary by Region?

Yes. North and West regions show higher median and spread than South and East.

Interpretation: Indicates potential for region-specific marketing or pricing strategies.

📊 Q7: Which Distribution Best Fits Sales_Amount?

Log-Normal fits best (visually better than Normal or Exponential).

Interpretation: Sales_Amount likely results from multiplicative factors, typical in real-world financial data.

📊 Q8: What % of Sales_Amount Lies Within 1 Standard Deviation?

58.60% falls within ±1σ from the mean.

Interpretation: Lower than the 68% expected in a normal distribution—supports non-normal behavior.

📊 Q9: Do New vs Returning Customers Differ in Sales_Amount?

Yes. Returning customers show higher median and more variation.

Interpretation: Loyal customers tend to buy more or buy higher-ticket items.

📊 Q10: Are There Outliers in Sales_Amount?

0 outliers detected using the IQR method.

Interpretation: The distribution is spread but doesn’t include extreme statistical outliers.
