# **Retail Sales Analysis and Insights**

## **Overview**

In today’s fast-paced and fiercely **competitive marketplace**, understanding customer behavior, sales performance, and product trends isn’t just valuable, **it’s vital for driving sustainable growth and gaining a competitive advantage**. This **Sales Analysis project** delivers a thorough, data-driven evaluation of transactional records to uncover impactful insights across time, geography, product categories, and consumer purchasing patterns.

By integrating **rigorous Exploratory Data Analysis (EDA) with advanced Machine Learning techniques**, the project goes beyond historical reporting to **provide predictive intelligence**, empowering businesses to refine sales strategies, enhance marketing ROI, and forecast future outcomes with greater accuracy. **The fusion of analytics and machine learning** is strategically designed to arm decision-makers with actionable insights that drive smarter, faster, and more strategic decisions, elevate customer engagement, maximize revenue potential, and maintain a competitive edge in an ever-evolving business landscape.


## **Goal of this Project**
The primary objective of this project is to **transform raw sales data** into actionable **business insights** that **fuel strategic, data-driven decision-making**. In an environment shaped by rising market complexities and evolving consumer expectations, it is no longer sufficient for businesses to merely understand historical performance—they must anticipate future trends and proactively prescribe optimal actions.

**This project aims to**:

- Uncover hidden sales patterns and identify untapped growth opportunities.

- Identify top-performing products and high-revenue cities driving business success.

- Analyze customer purchasing behavior to optimize the timing and targeting of marketing efforts.

- Forecast future sales trends to inform inventory management, budgeting, and strategic planning.

- Recommend targeted business strategies using customer segmentation and association rule insights.

**In simple terms: this project empowers stakeholders with the intelligence they need to make faster, smarter, and more strategic decisions—ultimately improving sales performance, streamlining operations, enhancing customer engagement, and driving profitability in a competitive landscape**.


## **The Business Challenge**
The business is currently facing challenges in understanding:

- Identifying which products or markets truly drive revenue.

- Lacking clarity on monthly or weekly sales performance trends.

- Not leveraging customer behavior timing to schedule marketing activities effectively.

- Being reactive rather than proactive in sales forecasting and planning.

- Missing opportunities in product bundling and targeted promotions.

- Without a clear understanding of these areas, the company risks inefficient spending, stock issues, and missed growth opportunities.

## **Business Questions**
This project aims to answer the following key questions:


1. Which month achieved the highest total sales, and what was the total sales figure recorded during that period?

2. What is the percentage growth in total monthly sales over time, and how does it vary across different months?

3. Which city achieved the highest total sales, and what was the total sales amount for that city?

4. Which product had the highest sales, and what factors do you believe contributed to its success? 

5. How do product sales vary across different days of the week, and what insights can be drawn from the distribution of order volumes by product and day?

6. On which day of the week do customers make the most purchases?

7. What is the optimal timing for advertisements and promotions to maximize customer purchases, based on historical purchase behavior?

8. What will our monthly sales look like over the next two years based on historical purchasing patterns?

9. What products are frequently bought together?

10. How can we group cities based on sales performance to uncover patterns for better sales strategy?


## **Methodology**
### **Phase I: EDA – Descriptive & Diagnostic Analysis**

**1.  Data Cleaning & Preprocessing**: Removing duplicates, handling missing values, creating more columns, and formatting     variables

**2.  Monthly Sales Analysis**: Identified the highest-grossing months and overall trends.

**3.  City-Level Analysis**: Mapped sales performance geographically.

**4.  Product & Weekly Trends**: Uncovered product demand patterns by weekday.

**5.  Insights Visualization**: Created clear visuals (bar charts, heatmaps) for storytelling.

### **Phase II: Machine Learning – Predictive & Prescriptive Models**

**1.  Time Series Analysis**: Determined optimal times for promotions and customer engagement.

**2.  Sales Forecasting**: Used Prophet models to predict future sales.

**3.  Market Basket Analysis**: Revealed frequent product pairings using Apriori algorithm or any other analysis.

**4.  Clustering**: Applied KMeans to segment cities for targeted sales strategies.

This phased approach ensures a solid foundation of insight (what and why) followed by predictive and strategic guidance (what’s next and how to act).


## **Tools & Technologies Used**

To explore the data analyst job market in depth, I utilized a robust set of tools and libraries that supported data analysis, visualization, and predictive modeling:

**1.  Python**: The foundation of my analysis, enabling efficient data manipulation and insight extraction. Key libraries included:

-	**Pandas** for data cleaning and analysis

-	**Matplotlib** for basic data visualizations

-	**Seaborn** for enhanced and detailed plotting


**2.  Machine Learning**: To uncover patterns and make predictive insights, I incorporated:

-	**scikit-learn** for model development and evaluation

-	**XGBoost** for high-performance gradient boosting

-	**Prophet** for time series forecasting

**3.  Jupyter Notebooks**: Provided an interactive coding environment, allowing for seamless integration of code, analysis, and documentation.

**4.  Git & GitHub**: Used for version control, code management, and collaboration, ensuring transparency and reproducibility throughout the project.


# **The Analysis**

# **I. Exploratory Data Analysis (EDA)**

# **1. Monthly Sales Performance Analysis**

## **Which month achieved the highest total sales, and what was the total sales figure recorded during that period**?

[Code & Other Resources - Monthly Sales Performance Analysis](https://github.com/olumidebalogun1/Retail-Sales-Analysis-and-Insights/blob/main/1.%20Monthly%20Sales%20Performance%20Analysis.ipynb): The complete code encompasses all stages of the project, from the initial **overview, goals, and business challenges to the methodology, data loading, cleaning, and formatting**. **It also includes visualizations, key insights, and strategic recommendations**

## **Result**

![1  Monthly Sales Performance Analysis](https://github.com/user-attachments/assets/8f549c25-5f5d-4433-8364-65e4939c39b2)


## **Key Insights**
1.	December recorded the highest total sales, with a revenue of $6,404,121.28, making it the most profitable month of the year.
2.	November followed as the second-highest month with $5,743,349.24, indicating a strong year-end sales trend.
3.	February was the weakest month, with the lowest total sales of $1,235,017.71.
A noticeable sales surge begins from June onward, suggesting a buildup toward the end-of-year peak.



# **2. Monthly Sales Growth Analysis**

## **What is the percentage growth in total monthly sales over time, and how does it vary across different months**?

[ Code & Other Resources - Monthly Sales Growth Analysis](https://github.com/olumidebalogun1/Retail-Sales-Analysis-and-Insights/blob/main/2.%20Monthly%20Sales%20Growth%20Analysis.ipynb): The complete code encompasses all stages of the project—from the initial **overview, goals, and business challenges to the methodology, data loading, cleaning, and formatting**. **It also includes visualizations, key insights, and strategic recommendations**.

## **Result**

![2  Monthly Sales Growth Analysis](https://github.com/user-attachments/assets/54944a17-05f4-406d-b265-0b3882726438)


## **Key Insights**
1.	High Volatility in Monthly Sales: The growth rates fluctuate significantly, with both steep declines (e.g., -73.38% in Month 2, -25.69% in Month 10) and sharp increases (e.g., +226.32% in Month 11, +90.99% in Month 23).
2.	Exceptional Growth in Month 11: The highest sales growth occurred in Month 11 (+226.32%), likely due to a seasonal or promotional event. This also marks the peak in total sales ($5.74M).
3.	Absolute peak occurred in Month 12 ($6.40M) with sales growth of +11.51%.
4.	Sustained Growth Toward Year-End: Despite mid-year dips (Months 7 to 10), Months 11 and 12 show strong recovery and surpass all previous months in both growth and absolute sales.
5.	Underperformance Early in the Year: Month 2 experienced a dramatic -73.38% drop from Month 1, suggesting either a data anomaly or external factor disrupting sales continuity.



# **3. Geographic Sales Analysis**

## **Which city achieved the highest total sales, and what was the total sales amount for that city**?

[Code & Other Resources - Geographic Sales Analysis](https://github.com/olumidebalogun1/Retail-Sales-Analysis-and-Insights/blob/main/3.%20Geographic%20Sales%20Analysis.ipynb): The complete code encompasses all stages of the project—from the initial **overview, goals, and business challenges to the methodology, data loading, cleaning, and formatting**. **It also includes visualizations, key insights, and strategic recommendations**.

## **Result**

![3  Geographic Sales Analysis](https://github.com/user-attachments/assets/f844e965-111f-4b83-b746-5d333700a687)


## **Key Insights**
1.	San Francisco (CA) recorded the highest total sales, pulling in approximately $9.39M, significantly outpacing all other cities.

2.	Los Angeles (CA) and New York City (NY) followed with $6.34M and $5.2M respectively, making California and New York powerhouses of revenue generation.

3.	Portland (ME) posted the lowest total sales at $541K, over 17x lower than San Francisco.
There is a notable performance gap between top-tier and mid/lower-tier cities. Cities like Austin (TX), Portland (OR), and Seattle (WA) are in the mid-range, suggesting room for growth.


# **4. Product Analysis**

## **Which product had the highest sales, and what factors do you believe contributed to its success**? 

[Code & Other Resources - Product Analysis](https://github.com/olumidebalogun1/Retail-Sales-Analysis-and-Insights/blob/main/4.%20Product%20Analysis.ipynb): The complete code encompasses all stages of the project—from the initial **overview, goals, and business challenges to the methodology, data loading, cleaning, and formatting**. **It also includes visualizations, key insights, and strategic recommendations**.

## **Result**

![4  Product Analysis1](https://github.com/user-attachments/assets/c1a2c74e-8c0d-45c1-8477-78ddabe6cab4)

![4  Product Analysis2](https://github.com/user-attachments/assets/2a9f717e-5b07-46c6-96ec-e0d7bd1cd004)


## **Key Insights**
1.	Top-Selling Product: AAA Batteries (4-pack) lead the pack with 23,970 units sold, closely followed by AA Batteries (4-pack) and USB-C Charging Cables.
2.	Accessory Dominance: The top 5 products are all low-cost, high-demand accessories (batteries, cables, headphones) rather than high-ticket items like phones or laptops.
3.	Price vs. Volume Trend: Low-cost items significantly outperform premium electronics in volume sold. For example, AAA Batteries outsold the iPhone nearly 4x and the MacBook Pro 5.5x.
4.	Brand Appeal in Audio: In the headphone category, Galaxy Buds outperform Apple Airpods and Bose SoundSport, suggesting strong market preference or price-value advantage.
5.	Low Sales in High-Value Appliances: Items like Amana Dryers and Washing Machines had the lowest sales, indicating either limited demand, higher price sensitivity, or fewer purchase occasions.


# **5. Product Sales Performance Analysis**

## **How do product sales vary across different days of the week, and what insights can be drawn from the distribution of order volumes by product and day**?

[ Code & Other Resources - Product Sales Performance Analysis](https://github.com/olumidebalogun1/Retail-Sales-Analysis-and-Insights/blob/main/5.%20Product%20Sales%20Performance%20Analysis.ipynb): The complete code encompasses all stages of the project—from the initial **overview, goals, and business challenges to the methodology, data loading, cleaning, and formatting**. **It also includes visualizations, key insights, and strategic recommendations**.

## **Result**

![5  Product Sales Performance Analysis](https://github.com/user-attachments/assets/69940a46-0f54-449e-90d9-43f48d130de0)


## **Key Insights**
1.	High-Demand Essentials Stay Consistent All Week: AAA & AA Batteries, Lightning/USB-C Charging Cables, and Galaxy Buds maintain consistently high sales across all days — essential, everyday items with minimal day-of-week fluctuation.
2.	Headphones Show Slight Weekend Preference: Apple Airpods, Galaxy Buds, and Bose Headphones see mild sales bumps on weekends (Sat–Sun) — likely driven by leisure time, gifting, or casual shopping.
3.	Monitors & Laptops Lean Toward Early Week Activity: Alienware, LG UltraGear, and Samsung Odyssey Monitors show slightly better performance on Mondays and Tuesdays, possibly reflecting corporate or productivity-driven purchases.
4.	Smartphones Steady but Subtle Decline Midweek: Products like iPhone, Google Phone, and Samsung Galaxy display more stable demand, though there's a minor dip midweek (especially for iPhones on Wed: 814, the lowest).
5.	Large Appliances Are Low Volume Overall: Amana Dryers & Washing Machines have low sales throughout the week, with slightly better traction on Mondays, which might suggest weekend browsing and Monday decision-making.
6.	Weekend Electronics Spike: Flatscreen TVs and Dell UltraSharp Monitors peak subtly on Sunday (TV: 604 → 898 for monitor), pointing to consumer behavior around weekend entertainment or research-buying patterns.


# **6. Weekly Purchase Trends Analysis**

## **On which day of the week do customers make the most purchases**?

[ Code & Other Resources - Weekly Purchase Trends Analysis](https://github.com/olumidebalogun1/Retail-Sales-Analysis-and-Insights/blob/main/6.%20Weekly%20Purchase%20Trends%20Analysis.ipynb): The complete code encompasses all stages of the project—from the initial **overview, goals, and business challenges to the methodology, data loading, cleaning, and formatting**. **It also includes visualizations, key insights, and strategic recommendations**.

## **Result**

![6  Weekly Purchase Trends Analysis](https://github.com/user-attachments/assets/b28acf77-62fb-4c59-b165-21354941bc9e)


## **Key Insights**
1.	Tuesday is the peak day for customer purchases, bringing in the highest total sales of $5.75M.

2.	Friday and Sunday closely follow as strong performers, with sales of $5.70M and $5.66M, respectively.


3.	Thursday records the lowest sales volume of the week at $5.41M, suggesting it’s the least active day for purchases.

4.	Overall, weekday performance is fairly balanced, with a slight edge on early and late-week days (Tue & Fri).


5.	Weekends (Sat & Sun) remain strong, especially Sunday with $5.66M, which may reflect increased leisure-time shopping behavior.


# **II. Machine Learning**

# **7. Time Series Analysis (Customer Behavior Timing)**

## **What is the optimal timing for advertisements and promotions to maximize customer purchases, based on historical purchase behavior**?

[Code & Other Resources - Time Series Analysis (Customer Behavior Timing)](https://github.com/olumidebalogun1/Retail-Sales-Analysis-and-Insights/blob/main/7.%20Time%20Series%20Analysis%20(Customer%20Behavior%20Timing).ipynb): The complete code encompasses all stages of the project—from the initial **overview, goals, and business challenges to the methodology, data loading, cleaning, and formatting**. **It also includes visualizations, key insights, and strategic recommendations**.

## **Result**

![7  Time Series Analysis (Customer Behavior Timing)](https://github.com/user-attachments/assets/78ac8729-320d-4586-b8b3-3ed52923bc51)


## **Key Insights**
1.	Customer activity follows a clear daily rhythm, starting low in the early morning, building momentum mid-morning, peaking in the afternoon and early evening, and tapering off gradually at night.
2.	Consistently high customer activity is observed between 11:00 AM and 9:00 PM, with the most significant spikes from:
•	11:00 AM to 2:00 PM (Peak hours: 11 AM – 11,393; 12 PM – 11,594; 1 PM – 11,207)
•	6:00 PM to 8:00 PM (Evening peak: 6 PM – 11,146; 7 PM – 11,757; 8 PM – 11,507)
3.	Low engagement periods are between 2:00 AM and 6:00 AM, where customer activity is minimal.


# **8. Sales Forecasting Using Prophet Mode**

## **What will our monthly sales look like over the next two years based on historical purchasing patterns**?

[Code & Other Resources - Sales Forecasting Using Prophet Model](https://github.com/olumidebalogun1/Retail-Sales-Analysis-and-Insights/blob/main/8.%20Sales%20Forecasting%20Using%20Using%20Prophet%20Model.ipynb): The complete code covers all stages of the project—from the initial **overview, goals, and business challenges to the methodology, data loading, cleaning, and formatting**. **It also includes the code used to train the Prophet model, along with visualizations, key insights, and strategic recommendations**.

## **Result**

![8  Sales Forecasting Using Using Prophet Model](https://github.com/user-attachments/assets/a690ae99-b8c3-4240-acfe-395913de83d3)


## **Key Insights**
1.	Consistent Upward Sales Trend: Forecasted monthly sales exhibit a steady upward trajectory, reflecting strong positive momentum in overall business performance.
2.	Average Monthly Growth: The model predicts an average monthly increase of approximately $40K–$50K, indicating healthy organic growth and potentially rising customer demand or market expansion.
3.	Seasonality Detected: While Prophet accounts for seasonal patterns, the confidence intervals show noticeable fluctuations around key months—likely due to holidays or promotion-driven spikes (e.g., November–December).
4.	Wide Confidence Intervals: The forecast shows broad prediction intervals in the near term (e.g., February–April 2025), indicating short-term volatility or uncertainty. These intervals narrow over time as more data becomes available.
5.	Strong Lower Bound: Even under conservative scenarios (lower bound estimates), monthly sales remain well above $1M, providing a reliable baseline for financial planning and inventory decisions.



# **9. Market Basket Analysis (Customer Purchase Behavior)**

## **What products are frequently bought together**?

[Code & Other Resources - Market Basket Analysis (Customer Purchase Behavior](https://github.com/olumidebalogun1/Retail-Sales-Analysis-and-Insights/blob/main/9.%20Market%20Basket%20Analysis%20(Customer%20Purchase%20Behavior).ipynb): The complete code encompasses all stages of the project—from the initial **overview, goals, and business challenges to the methodology, data loading, cleaning, and formatting**. **It also includes visualizations, key insights, and strategic recommendations**.

## **Result**

### **Top 20 product pairs most frequently ordered together**

![9 0 Market Basket Analysis (Customer Purchase Behavior)](https://github.com/user-attachments/assets/6746d406-5470-416f-b8a5-894e9d765b25)

### **Top 10 sets of three (3) products most commonly ordered together**

![9 1 Market Basket Analysis 2](https://github.com/user-attachments/assets/2971291e-54aa-4b01-a231-89f38cef47d5)


## **Key Insights**
1.	Strong Accessory Dependency:
•	iPhone is frequently bought with the Lightning Charging Cable (473 times) and Apple AirPods Headphones (173 times), confirming a strong dependency on accessories.
•	Similar behavior observed for Google Phone and USB-C Charging Cable (469 times), and Samsung Galaxy Phone with the same cable (177 times).
2.	Bundling Behavior Around Devices:
•	Buyers often purchase phones with multiple accessories (e.g., Google Phone + USB-C Cable + Headphones combinations).
•	Example: Google Phone + USB-C Charging Cable + Bose SoundSport Headphones is a top 3-product combo.
3.	Cross-Brand Headphone Love:
•	Galaxy Buds Headphones appear frequently with iPhone, Google Phone, and Samsung Galaxy Phone, suggesting customers aren't loyal to brand-specific headphones. They mix and match based on price, design, or preference.
4.	Repetitive Combination Patterns:
•	Most of the high-frequency combinations are symmetrical (e.g., iPhone + Lightning Cable and Lightning Cable + iPhone)—reinforcing the reliability of the insight.
5.	Accessory-Driven Purchases:
•	Accessories like charging cables and headphones dominate the co-purchase behavior. These aren’t just afterthoughts—they're clearly planned purchases.


# **10. Clustering Cities Using the KMeans Mode**

## **How can we group cities based on sales performance to uncover patterns for better sales strategy**?

[Code & Other Resources - Clustering Cities Using the KMeans Model](https://github.com/olumidebalogun1/Retail-Sales-Analysis-and-Insights/blob/main/10.%20Clustering%20Cities%20Using%20the%20KMeans%20Model.ipynb): The complete code covers all stages of the project—from the initial **overview, goals, and business challenges to the methodology, data loading, cleaning, and formatting**. **It also includes the code used to train the KMeans model, along with visualizations, key insights, and strategic recommendations**.

## **Result**

![10  Clustering Cities Using the KMeans Model](https://github.com/user-attachments/assets/5c32899c-0726-4098-a9b3-4bcf97293a22)


## **Key Insights**
1. Cluster 0 – High Sales & High Volume Cities
Interpretation:
•	Cities in this cluster show strong performance in both revenue and unit sales.
•	Indicates high demand, strong customer base, and effective local execution.

2. Cluster 1 – Moderate Sales & Moderate Volume Cities
Interpretation:
•	These cities perform reasonably well but have room for growth.
•	Represents stable markets with potential to be moved into the high-performing cluster.

3. Cluster 2 – Low Sales & Low Volume Cities
Interpretation:
•	Underperforming regions with low revenue and low units sold.
•	Maybe an indication of market saturation, low demand, or ineffective sales presence.



# **Key Expected Result and Estimated Business Impact**

### **Expected Result**:
Strategic optimization of sales timing, regional focus, product bundling, and marketing execution is projected to drive **12–22% revenue growth**, **6–14% increase in profit margins**, and **8–18% uplift in customer engagement and retention**.

### **Estimated Business Impact**:
**1. Revenue Growth**: **+12–22%** through enhanced Q4 campaigns, product bundling, and targeted promotions aligned with peak sales periods and high-performing cities.

**2. Profit Margin Improvement**: **+6–14%** via increased sales of high-margin accessories, operational efficiency from better forecasting, and inventory alignment with demand.

**3. Customer Retention**: **+8–18%** through improved cross-selling, loyalty initiatives in top-tier markets, and personalized weekday/time-based engagement strategies.

**4. Cost Optimization**: **+7–12%** reduction in operational waste through data-driven inventory and staffing planning based on forecasted demand and customer behavior trends.

**5. Marketing ROI**: **+10–20%** by focusing efforts on high-impact times (Tuesdays, 11 AM–2 PM), channels (bundling/cross-promotion), and locations (top-revenue cities).

**6. Market Penetration**: **Up to +9%** increase in underperforming regional sales via localized strategies, geo-targeted offers, and cluster-specific campaigns.


## **What I Learned**
Throughout this project, I significantly deepened my understanding of **Retail Sales Analysis** and strengthened my technical expertise in **Python-based data analytics and machine learning**. Here are some of the most valuable skills and insights I gained:

-	**Advanced Python Skills**: I enhanced my ability to manipulate and analyze data using libraries such as **Pandas**, while leveraging Matplotlib and Seaborn for effective visual storytelling.

-	**Machine Learning Application**: I applied models using **Scikit-learn, XGBoost**, and **Prophet** to identify patterns and generate predictive insights, moving beyond descriptive analytics to deliver strategic foresight.

-	**Data Cleaning & Preparation**: I reinforced the importance of meticulous data cleaning and formatting as the foundation for accurate, reliable analysis and model performance.

-	**Strategic Insight Generation**: By combining EDA with machine learning techniques, I learned how to generate business-critical insights that inform strategy, optimize marketing efforts, and support forward-looking decision-making.

## **Challenges & Growth**
This project came with its share of challenges, each providing valuable opportunities for growth:

-	**Handling Data Inconsistencies**: Navigating missing, duplicated, or inconsistent entries sharpened my data preprocessing techniques and taught me how vital data integrity is to meaningful analysis.

-	**Complex Visualizations**: Translating dense, multi-dimensional data into intuitive and impactful visualizations required creativity and precision—skills I significantly improved through iteration.

-	**Balancing Detail and Scope**: Striking the right balance between diving deep into specific analyses and maintaining a broad strategic overview was a continuous learning process, enhancing my ability to manage project scope effectively.


## **Conclusion**
This Retail Sales Analysis and Insight project showcases how combining Exploratory Data Analysis with Machine Learning can turn raw sales data into clear, actionable strategies. By uncovering sales patterns across time, geography, and customer behavior, the project addresses critical business questions, such as top-performing months, cities, and products, while revealing opportunities in product bundling, promotion timing, and customer segmentation.
Advanced techniques like **Prophet forecasting, market basket analysis**, and **KMeans clustering** provided predictive power and strategic guidance, enabling smarter decisions in inventory, marketing, and planning.

In short, this project equips decision-makers with the insights needed to optimize performance, enhance customer engagement, and drive sustained growth in a competitive retail environment.


**Feel free to explore, share, and connect! Let's transform data into decisions that drive measurable impact**.

## **Connect with Me**
- **📞 +234-8065060691**
- **📧 Email: Olumide Balogun**
- **🔗 LinkedIn**: [Connect with me on LinkedIn](https://www.linkedin.com/in/olumide-balogun1/)
- **🔗 Medium**: [Explore my Data Storytelling articles](https://medium.com/@Olumide-Balogun)

